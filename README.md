# Gen NFT Art

A Python project for generating stylized NFT artwork from layered visual assets. The generator composes background images, character portraits, textured overlays, and retro-styled text into high-resolution PNG outputs suitable for NFT collection experimentation and artistic exploration.

## Overview

This project builds unique visual compositions by combining images from the `images/` directory and applying geometric overlays, rotated typography, and a retro gaming aesthetic. It is designed as a lightweight generator for creating collection-ready artwork variants.

## Features

- Layer-based artwork composition
- Character and background image blending
- Vertical and diagonal decorative overlays
- Retro-inspired text rendering using a custom font
- High-resolution output generation at 2000 x 2000
- Easy extension for additional generation templates

## Project Structure

```text
gen-nft-art-master/
├── nft_gen.py              # Main generator script
├── Retro Gaming.ttf       # Font used for text layers
├── images/
│   ├── backdrop/
│   ├── individual/
│   └── verticalLines/
├── output/                 # Generated PNG files (created during runtime)
├── README.md
└── .git/
```

## Requirements

- Python 3.8+
- Pillow (`PIL`)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/gen-nft-art.git
cd gen-nft-art
```

2. Create and activate a virtual environment (optional but recommended):

```bash
python -m venv .venv
source .venv/bin/activate   # Linux/macOS
.venv\Scripts\activate      # Windows
```

3. Install dependencies:

```bash
pip install pillow
```

## Usage

Run the generator:

```bash
python nft_gen.py
```

The script currently generates sample output using pre-defined image assets and saves them into the `output/` directory. You can modify the generation logic inside `nft_gen.py` to change text, asset selection, and output patterns.

## Customization

The script is structured around several generation functions:

- `generateParcel1(...)`
- `generateParcel2(...)`
- `generateParcel3(...)`
- `generateParcel4(...)`

Each function assembles a different visual style by combining a background, an individual image, and overlay effects. You can edit the text value, generation loop, or asset filters to produce varied collections.

## Output

Generated files are stored in the `output/` folder using names such as:

```text
output/parcel1/0.png
output/parcel2/0.png
output/parcel3/0.png
output/parcel4/0.png
```

## Notes

- The project relies on the included `Retro Gaming.ttf` font.
- Asset directories should remain organized under `images/` to ensure the generator can load files correctly.
- If you plan to generate a large NFT collection, consider expanding the asset pool and automating naming conventions.

## License

This project is provided for educational and creative use. Please review and comply with the relevant terms for any assets used in the generated artwork.

## Contributing

Contributions are welcome. If you improve the generation pipeline, add new templates, or optimize the art generation flow, feel free to submit a pull request.
