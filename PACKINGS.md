# Square-packing certificates — Kaelan Yim

Exact rational witnesses of AI-assisted computational refinements. These are upper-bound certificates, not optimality proofs or blanket claims of current public records. Earlier constructors, source holders and method authors retain their credit; per-certificate lineage is in `packing-certificates.json` and the original certificate comments. Do not credit these as independent original constructions.

The existing `n260.cert` and profile README are unchanged. Its earlier registry result is T-265 (now historical/superseded).

## Certificate snapshot

Sides below are **rounded upward to 12 decimal places** for display only. The exact rational side in each certificate and manifest is authoritative.

| n | Certificate | Upper bound (rounded upward) |
|---:|---|---:|
| 130 | [n130.cert](n130.cert) | 11.902430645983 |
| 299 | [n299.cert](n299.cert) | 17.801004434255 |
| 303 | [n303.cert](n303.cert) | 17.901789273154 |
| 553 | [n553.cert](n553.cert) | 23.969145238668 |
| 599 | [n599.cert](n599.cert) | 24.936479681246 |
| 600 | [n600.cert](n600.cert) | 24.951090275321 |
| 601 | [n601.cert](n601.cert) | 24.958070476928 |
| 602 | [n602.cert](n602.cert) | 24.981298949631 |
| 604 | [n604.cert](n604.cert) | 24.995880488226 |
| 645 | [n645.cert](n645.cert) | 25.881385537401 |
| 647 | [n647.cert](n647.cert) | 25.899272968790 |
| 648 | [n648.cert](n648.cert) | 25.908803576981 |
| 699 | [n699.cert](n699.cert) | 26.907311118315 |
| 700 | [n700.cert](n700.cert) | 26.908036102718 |

**n130 is an archival envelope-only variant:** side `11.9024306459822462042030375294435824…` (upward to 16 places: `11.9024306459822463`), approximately `1.9554409882111e-14` below the source certificate. Every relative center and orientation is unchanged; only a common translation and the containing-box size change. This is **not a new packing or numerical search gain**. The [maintainer discussion](https://github.com/jlevy/squares/issues/846#issuecomment-6543941452) distinguishes padding-only re-certifications and raises their eligibility inside the Atlas range; **no Atlas credit is claimed or recommended from this file**. The source’s MIT [copyright/permission notice](n130-source-LICENSE.txt) and ancestry are retained. A byte-identical [text copy](n130.cert.txt) is included.

**n299 is a verified microscopic tightening:** the exact side is `17.80100443425411170800278978866085574955…`, smaller than the pending [Doğa Özden #929](https://github.com/jlevy/squares/issues/929) witness by approximately `1.1819655270744e-12`. It comes from returned-anchor continuation, not either broader kick. This is a refinement of his arrangement, not a new construction or material gain. Requested further-refinement credit: **Kaelan Yim after Doğa Özden, Evan Daniel and Chris Deotte**. Acceptance and Atlas credit remain the maintainers’ decision. A byte-identical [text copy](n299.cert.txt) is available for attachment hosts.

**n303 now has a verified microscopic refinement:** exact side `17.9017892731531992856633983391691014…`, approximately `3.2910456934182e-12` below the pinned [Doğa Özden #930](https://github.com/jlevy/squares/issues/930) witness. It came from the **no-strain control**, not the aspect-strain proposal (which recovered worse). Relative centers change microscopically; this is not merely a common translation/reboxing, but neither a structural nor material improvement. Credit: **Kaelan Yim after Doğa Özden, Evan Daniel, Chris Deotte and Griffin Casson**. The source [license declaration](n303-source-LICENSE.md) and a byte-identical [text copy](n303.cert.txt) are included. **Protocol qualification:** the pre-science pair-Jacobian fixture accidentally tested only walls; the later full pair check passed but does not retroactively cure admission. Five exact geometry checks passed separately; independent cohort review remains pending. The original material milestone remains unmet. Atlas acceptance/credit are not guaranteed. The current visual Atlas covers n=1..324; higher-count files are outside that display.

## Reproduce exact feasibility checks

The two public checker files below are byte-identical to the copies used for the recorded checks. They share an author and input format, but use different geometry tests. Together with the local rational repair verifier and the registry center/basis and independent-corner routes, five local exact checks accepted every new certificate. These are not five wholly independent implementations.

```sh
git clone https://github.com/evand/square-packing.git
cd square-packing
git checkout bb4cc78e5b35103c1f177db55e9cf08974e66563
python3 search/exact/verify_cert.py /path/to/n303.cert
python3 search/exact/verify_cert2.py /path/to/n303.cert
```

Replace `n303.cert` with any certificate to check. Checker SHA-256 values:

- `verify_cert.py`: `3299ca0c0f02f7c221deeea69a9a85b5a90db6bc410b20727fdff211c92bed52`
- `verify_cert2.py`: `55140a35d95d9eaa64a14c3b044641efbcda94ebfc3b12b7dec9fa52692e31d3`

Run `sha256sum -c SHA256SUMS` from this repository to check file identity, including the pre-existing n260 certificate, byte-identical n130/n299/n303 text copies, and the n130 upstream license notice. Certificates are copied byte-for-byte from the verified local releases; historical comments containing “private” describe their pre-publication status.

## Submission and attribution

Requested improvement credit: **Kaelan Yim** (GitHub `vitamoon`). AI assistance: Hermes Agent was used for research, numerical search, implementation and verification orchestration. Full prior construction/method lineage must accompany a submission. In particular, n303 refines Doğa Özden after Evan Daniel and Chris Deotte, with Griffin Casson’s recovery solver; n604 builds on Couzo/alexchilton work. Other source credits are retained per certificate. No sole-inventor or priority claim is made.

Publishing certificates here is not an Atlas registration. Use a full commit URL and the SHA-256 in `packing-certificates.json` when reporting a result. The repository owner submits registration requests; none were posted by this publication step.

The prior n260 license statement remains specific to that file. This snapshot makes no blanket new license assertion for inherited third-party materials; their attribution and licensing constraints remain applicable.
