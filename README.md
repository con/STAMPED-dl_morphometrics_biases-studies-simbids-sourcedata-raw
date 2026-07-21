# Three-subject SimBIDS raw fixture

This independent DataLad dataset contains three synthetic participants and no
human observations or identifiers. SimBIDS `0.1.dev27+g1a8efa3` created the
BIDS skeleton using `code/phase3-three-subjects.yaml` in the exact SIF with
SHA-256 `244af4c6e1708dc10dd1f89f28951c9efa1c01571de778449ed4593ef8e9bbea`.

SimBIDS creates zero-byte imaging placeholders; its `--fill-files` option writes
random bytes rather than NIfTI. The root project therefore ran the tracked
`scripts/materialize_simbids_niftis.py` with nibabel 5.3.3 and NumPy 1.26.4 to
create deterministic valid tiny images. This is engineering test data for a
three-job BABS qualification, not scientifically meaningful MRI.
