# AI_Presentation_Generator
# AI Presentation Generator

This project creates a PowerPoint presentation with slides that include enhanced content and images generated using OpenAI's API.

## Features

- Generates detailed explanations for slide content using GPT-3.5-turbo.
- Creates images for slides using DALL·E 3.
- Compiles the slides into a PowerPoint presentation.

## Prerequisites

- Python 3.7+
- OpenAI API Key

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/AI_Presentation_Generator.git
    cd AI_Presentation_Generator
    ```

2. Create and activate a virtual environment:

    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4. Create a `.env` file in the root directory of the project and add your OpenAI API key:

    ```plaintext
    OPENAI_API_KEY=your_api_key_here
    ```

## Usage

1. Modify the `slides` list in the script to include the slides you want to create:

    ```python
    slides = [
        {
            "title": "Introduction to AI",
            "content": "Artificial Intelligence (AI) is the simulation of human intelligence in machines...",
            "image_prompt": "A futuristic robot interacting with humans"
        },
        {
            "title": "Applications of AI",
            "content": "AI has numerous applications including healthcare, finance, transportation, and more...",
            "image_prompt": "AI in healthcare, finance, and transportation"
        },
        # Add more slides as needed
    ]
    ```

2. Run the script:

    ```bash
    python generate_presentation.py
    ```

3. The PowerPoint presentation `AI_Presentation.pptx` will be created in the project directory.

## Example

Here is an example of how to use the script:

```bash
$ python generate_presentation.py
Loaded API Key: your_api_key_here
Presentation created successfully!
