# Universal Paper Analyzer

Analyze scientific papers using OpenAI GPT models. This tool extracts text from PDF files and analyzes them based on a customizable prompt template. It is designed for researchers, students, and interdisciplinary thinkers who want to quickly extract insights from complex scientific documents.

## Features

* **Flexible PDF Text Extraction:** Efficiently extracts text from multi-page PDF files.
* **Token Management:** Automatically splits text into manageable chunks for OpenAI models.
* **Parallel Processing:** Speeds up analysis with multithreading.
* **Customizable Templates:** Easily modify the prompt for different types of papers.
* **Error Handling:** Provides clear error messages for missing files and unsupported formats.

## Installation

Clone this repository and install the required packages:

```bash
git clone https://github.com/yourusername/Paper-Analysis-Tool.git
cd Paper-Analysis-Tool
pip install -r requirements.txt
```

## Setup

Create a `.env` file in the project root and add your OpenAI API key:

```
OPENAI_API_KEY=your-api-key-here
```

## Usage

Run the script from the command line with the path to the PDF file:

```bash
python paper_analysis.py "/path/to/your/paper.pdf"
```

## Requirements

* Python 3.8+
* OpenAI API Key
* Required Packages:

  * langchain-openai
  * python-dotenv
  * PyMuPDF

## Customization

You can easily modify the analysis template in the `paper_analysis.py` file:

```python
PROMPT_TEMPLATE = '''Analysiere das Paper anhand der folgenden fünf Prinzipien:
1. Systemische Definition (Zentrale Fragen und Ziele)
2. Interdisziplinarität (Beteiligte Disziplinen)
3. Deep Data & Vernetzung (Wichtige Datenquellen)
4. Mustererkennung (Zentrale Muster und Mechanismen)
5. Validierung & Kreativität (Kritische Punkte und Innovationen)'''
```

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue if you find a bug or have a feature request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
