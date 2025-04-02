# NFT Generator

A Python-based automation script designed to streamline the creation of NFTs using various image layers.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Metadata Generation](#metadata-generation)
- [Output](#output)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Overview

NFT Generator automates the process of creating unique Non-Fungible Tokens (NFTs) by combining different image layers. This tool is ideal for artists and developers looking to produce large collections of NFTs efficiently.

## Features

- **Layer-Based Image Composition**: Combine multiple image layers to create unique NFT artworks.
- **Automated Metadata Generation**: Produce metadata compatible with NFT standards.
- **Customizable Rarity Settings**: Define the rarity of specific traits or layers.
- **Batch Processing**: Generate multiple NFTs in a single run.

## Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/siddhiipatell/NFT-Generator.git
   ```

2. **Navigate to the Project Directory**:

   ```bash
   cd NFT-Generator
   ```

3. **Install Required Dependencies**:

   Ensure you have Python installed. Then, install the necessary packages:

   ```bash
   pip install -r requirements.txt
   ```

   *(Note: The `requirements.txt` file should list all necessary Python packages. If it's missing, please refer to the project's documentation or source code for dependencies.)*

## Usage

1. **Prepare Your Assets**:

   - Organize your image layers into folders within the `assets` directory. Each folder represents a trait category (e.g., Backgrounds, Bodies, Accessories).

2. **Configure the Generator**:

   - Adjust settings in the `config.py` file to define output directories, image dimensions, and other parameters.

3. **Run the Script**:

   Execute the main script to start generating NFTs:

   ```bash
   python nft.py
   ```

4. **Review Outputs**:

   - Generated images will be saved in the `output` directory.
   - Corresponding metadata files will be stored as specified in your configuration.

## Configuration

The `config.py` file allows you to customize various aspects of the NFT generation process:

- **Output Directory**: Specify where generated images and metadata should be saved.
- **Image Dimensions**: Set the width and height for the output images.
- **Rarity Weights**: Define the probability of each layer or trait appearing in the final NFTs.

Example snippet from `config.py`:

```python
OUTPUT_DIR = './output'
IMAGE_SIZE = (500, 500)
RARITY_WEIGHTS = {
    'Backgrounds': {'Blue': 50, 'Red': 30, 'Green': 20},
    'Bodies': {'Alien': 70, 'Robot': 30},
    # Add other trait categories and their weights
}
```

## Metadata Generation

The script includes functionality to generate metadata for each NFT, aligning with common standards used in various NFT marketplaces. The `metadata.py` module handles this process, ensuring each NFT has a corresponding metadata file detailing its attributes.

## Output

After running the script, you'll find:

- **Images**: NFT artworks in the `output/images` directory.
- **Metadata**: JSON files containing attribute data in the `output/metadata` directory.

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch:

   ```bash
   git checkout -b feature-name
   ```

3. Make your changes and commit them:

   ```bash
   git commit -m "Description of changes"
   ```

4. Push to your forked repository:

   ```bash
   git push origin feature-name
   ```

5. Open a Pull Request detailing your changes.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgements

Special thanks to all contributors and the open-source community for their invaluable resources and support.

