# Rebuilding a private reference library

Use the [catalog](README.md) as bibliography, then record the exact copies that a
host can lawfully obtain. The directory convention is
`~/.local/share/<project>/library/`. This is a convention, not an installed path,
shared mount, storage service or permission grant. Each host resolves its own
project name and private storage. Nothing from the library is published or
committed: original files, manifests, hashes and rights records remain private.
The public catalog contains no host inventory or book content.

## MANIFEST.tsv

Use UTF-8 TSV with one header and one row per intended artifact. Header fields,
in order, are:

```text
id	kind	title	authors	edition/version	year	official_url	expected_licence	access	target_filename	notes
```

| Column | Meaning |
| --- | --- |
| `id` | Stable local artifact ID; retain the catalog ID in this ID or in notes. Split a chapter set into distinct artifact IDs. |
| `kind` | Artifact type, such as book, chapter or paper; distinguish a reading list from full text. |
| `title`, `authors` | Bibliographic identity of the actual work. Separate multiple authors with semicolons. |
| `edition/version`, `year` | Edition, revision/build or dated web snapshot and publication year; record unknowns explicitly. |
| `official_url` | Official acquisition URL for open/paid items, or exactly `owner-provided`. A paid landing page is not a direct full-text download. |
| `expected_licence` | Expected terms and their certainty; this field is a hypothesis to check, not authorization. |
| `access` | Exactly `open`, `paid` or `owner-provided`, describing the chosen lawful route. |
| `target_filename` | Unique basename within the library; no absolute path, parent traversal or control characters. |
| `notes` | Catalog ID, intended version, acquisition status, blocked reason, substitute and any rights/version uncertainty. |

Use no literal tab or newline inside a field; express such detail as ordinary
space-separated prose. Keep filenames distinct across editions. A substitute is
a separate artifact with its own identity, not bytes placed under the original
title's filename. Metadata-only and unavailable rows stay explicitly unavailable;
do not mark them acquired or give them a full-text checksum.

## SHA256SUMS

After verifying that a file is the intended full text and version, hash its exact
bytes. Use the standard `sha256sum` format: lowercase 64-character digest, two
spaces and the target basename. Record only files actually acquired; no invented
hashes and no abstract or error-page hashes passed off as books. Verify with
`sha256sum --check SHA256SUMS` before relying on that host's copies. A matching
hash establishes byte identity, not lawful access, correct edition, factual truth
or completed reading. Never edit the book bytes merely to normalize metadata;
record a new version and hash when the source changes.

## LICENSES.tsv

Use UTF-8 TSV with these header fields, in order:

```text
filename	sha256	source	licence	timestamp
```

| Column | Meaning |
| --- | --- |
| `filename` | Exact acquired basename, matching the manifest. |
| `sha256` | Same digest as SHA256SUMS, binding the rights observation to those bytes. |
| `source` | Actual official source and any permitted publisher-platform redirect, or `owner-provided`. Never store signed URLs, credentials or private download tokens. |
| `licence` | Observed terms, edition evidence, verification scope and unresolved limits. Retain expected/unknown status when not verified; free access alone is insufficient. |
| `timestamp` | UTC observation time in ISO 8601 format. |

Retain a new observation rather than erasing a prior acquisition's provenance.
Repeated observations of identical bytes must agree on identity; explain a rights
correction in the new record. A licence for editorial material does not cover all
included readings, figures, code or datasets.

## Acquisition rules

1. Start with the manifest identity and access route. Use official author,
   publisher or authorized project URLs only. No mirrors or paywall workarounds.
2. Inspect redirects before fetching. Do not follow a host-changing redirect
   except to the publisher's own platform. If an official page sends the file
   somewhere else, stop and record it unavailable under these rules; do not treat
   every linked CDN, archive or storage bucket as an approved destination.
3. For paid items, obtain a permitted purchase or loan, or select an open
   substitute. For owner-provided items, obtain an authorized private copy from
   the owner. Do not search for replacement download links or promise that
   another host can recover privately supplied bytes from a hash.
4. Check the response type, bibliographic identity, edition and completeness.
   Reject an abstract, preview, contents page, login page or error response as a
   replacement for full text. A legitimately chapter-split book uses distinct
   chapter rows and records missing chapters; do not claim a complete book from
   a subset.
5. Record actual source, observed licence/limits and timestamp in LICENSES.tsv;
   bind them to the same bytes as SHA256SUMS. Keep access failures and unknown
   terms explicit. Recheck before any proposed reuse beyond private reading.
6. Verify the acquired subset and report what remains unavailable. Rebuilding a
   library can reproduce organization and identities without obtaining every
   item; a new source revision needs a new record, never an assumed hash match.
7. Keep all library files and acquisition records private and outside version
   control. Publish no PDFs, book text, extracted passages or quotations. A
   project may separately maintain its own permitted bibliographic references,
   reading locators and original notes under its publication rules.
