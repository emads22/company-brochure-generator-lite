# Company Brochure Generator Lite

## Overview
The **Company Brochure Generator Lite** is a Python-based utility for creating professional, concise, or humorous brochures tailored for companies. By analyzing the content of a company's website, the tool extracts relevant information and uses the AI-powered open-source Ollama model `llama3.2` to format this data into user-friendly Markdown content. The brochures can serve prospective customers, investors, or recruits.

## Features
- **Website Content Extraction**: Scrapes and parses website content, including titles, text, and links, while excluding irrelevant elements.
- **Relevant Links Filtering**: Uses AI to identify and prioritize links, such as "About", "Careers", or "Company" pages, for inclusion in the brochure.
- **Brochure Generation**: Generates professional or humorous Markdown-formatted brochures using the Ollama model `llama3.2`.
- **Dynamic Streaming**: Displays the brochure content dynamically as it is being generated.
- **Standard Brochure Creation**: Allows users to generate the full brochure at once using the `create_brochure` function.

## Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/emads22/company-brochure-generator-lite.git
   cd company-brochure-generator-lite
   ```
2. Ensure Conda is installed.
3. Create the Conda environment using the provided `brochure_builder_env.yml` file:
   ```bash
   conda env create -f brochure_builder_env.yml
   conda activate brochure_builder
   ```
4. Configure the script to use the Ollama model `llama3.2` (ensure access to the model).
5. Optionally, adjust constants like `MODEL` and `HEADERS` in the script if necessary.
6. Launch Jupyter Lab:
   ```bash
   jupyter lab
7. Open the `brochure_builder_lite.ipynb` notebook in Jupyter Lab and run the cells step-by-step.

## Usage
1. Open Jupyter Lab and navigate to the `brochure_builder_lite.ipynb` notebook.
2. Run the notebook cells sequentially.
3. To create a brochure dynamically, use the `stream_brochure` function:
   ```python
   stream_brochure("Company Name", "https://companywebsite.com")
   ```
4. If you prefer not to stream the content, use the `create_brochure` function instead:
   ```python
   create_brochure("Company Name", "https://companywebsite.com")
   ```
5. Modify the `brochure_system_prompt` to change the tone of the brochure. For example:
    - Uncomment the humorous prompt in the script to generate a lighthearted, entertaining brochure.
    - Adjust the prompt text to suit your specific needs, such as focusing on particular aspects of the company or adopting a custom tone.
6. Results are dynamically displayed in the Jupyter Lab interface.

## Contributing
Contributions are welcome! Here are some ways you can contribute:
- Report bugs or issues.
- Suggest new features or improvements.
- Submit pull requests with bug fixes or enhancements.

## Author
- Emad &nbsp; E>

  [<img src="https://img.shields.io/badge/GitHub-Profile-blue?logo=github" width="150">](https://github.com/emads22)

## License
This project is licensed under the MIT License, which grants permission for free use, modification, distribution, and sublicense of the code, provided that the copyright notice (attributed to [emads22](https://github.com/emads22)) and permission notice are included in all copies or substantial portions of the software. This license is permissive and allows users to utilize the code for both commercial and non-commercial purposes.

Please see the [LICENSE](LICENSE) file for more details.

