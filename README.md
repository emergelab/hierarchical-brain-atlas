# hierarchical-brain-atlas

This repository keeps two organizations in parallel for pipeline compatibility.

## Layout

- Legacy layout (for older pipelines):
  - `legacy-spec/AA*/atlas-<atlas>_...`
- BIDS derived-atlas layout (for newer pipelines):
  - `bids-derived-atlas-spec/tpl-<space>/anat/tpl-<space>_atlas-<atlas>_<entities>_dseg.nii.gz`
  - `bids-derived-atlas-spec/tpl-<space>/anat/tpl-<space>_atlas-<atlas>_<entities>_dseg.json`

## Notes

- Atlas identifiers are preserved from the original release (for example: `AA7Parcels`, `AA50Parcels2mm`).
- Files aligned to different template spaces are grouped under the corresponding `tpl-<space>/` directory in `bids-derived-atlas-spec/`.
- Root-level `atlas-*` metadata files are intentionally omitted.