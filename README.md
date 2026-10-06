# ledger-anchors

External integrity anchors for the Silhouette signed receipt chain.

Each `anchors/seq-<N>.json` file pins one chain head: `seq`, `entryHash` (SHA-256 of the receipt payload) and `keyId` of the signer. One commit and one tag (`anchor-seq-<N>`) per anchored head. Hashes only: no receipt contents, no personal data.

Format, producer and verifier live in Silhouette-Agency-OS-OpenSource (`docs/RECEIPT_ANCHORS.md`: `chainHead`, `buildAnchor`, `verifyAnchor`). Boundary: single owner, single ledger, single repository.
