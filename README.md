# Enigma2 Addons Repository

## Structure
- `packages/`  put your `.ipk` files here
- `meta/`      one JSON per addon (category, Arabic description, supported images). File name = package name
- `icons/`     PNG icons
- `addons.json` generated index read by the panel plugin
- `tools/build_index.py` index generator

## Add an addon
1. Copy `name_1.0_all.ipk` into `packages/`
2. Create `meta/name.json` (copy `meta/example.json`)
3. Run: `python3 tools/build_index.py YOUR_USER YOUR_REPO`
4. Commit and push (or let the GitHub Action do step 3 automatically)

## Index URL for the plugin
https://raw.githubusercontent.com/YOUR_USER/YOUR_REPO/main/addons.json

Only upload packages you are allowed to redistribute.
