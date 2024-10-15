# Narrative ML + CLIP Integration
## Overview

This project aims to integrate NarrativeML annotations with OpenAI's CLIP model to process and analyze narrative structures in multimodal scenes. The repository contains XML-based narrative descriptions and Python scripts that utilize CLIP for understanding and interpreting these scenes, combining natural language processing and computer vision techniques.

The core objectives of this project are:
- Parsing narratives represented in XML format.
- Using CLIP to process visual content related to the narratives.
- Associating events, characters, and places described in text with corresponding visual elements in images or videos.

## Prerequisites

To run the scripts in this repository, ensure you have the following installed:
- Python 3.7+
- OpenAI's CLIP model
- PyTorch
- XML parsing libraries (e.g., `lxml`)
- Any additional Python dependencies listed in `requirements.txt`

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/narrative-ml-clip-integration.git
   cd narrative-ml-clip-integration
   ```

2. Create a virtual environment and activate it:

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Parsing NarrativeML Files

Use the `narrative_parser.py` script to parse XML files containing narrative annotations:

```bash
python scripts/narrative_parser.py --input-file GPT-4o-output.xml
```

### Running CLIP Integration

Once you've parsed the narrative annotations, you can run the CLIP integration script to link visual content with the narrative components:

```bash
python scripts/clip_integration.py --input narrative_output.json --image your-image-file.jpg
```

## Future Work

- Further integration of CLIP to process video content alongside textual narrative annotations.
- Extending the narrative schema to include more complex relationships between events, characters, and settings.

## License

This project is licensed under the MIT License.
