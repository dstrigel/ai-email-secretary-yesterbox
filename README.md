# AI Email Secretary (Yesterbox + LLM Automation)

The AI Email Secretary is a hands-on demonstration of applied generative AI, combining large language model reasoning, Yesterbox-style prioritization, and structured JSON evaluation to help users organize and act on incoming email with minimal effort.

This project simulates a real-world workflow: fetching messages, filtering them by date, classifying their urgency and action requirements, and generating executive-level summaries. The implementation includes prompt engineering, error handling, and automated scoring of results using LLM-as-Judge logic.

---

## Features

### Email Intake and Filtering
- Automatically identifies “yesterday’s” messages by parsing the filename pattern  
- Implements Yesterbox-style triage: urgent, deadline-driven, high-priority, low-priority, FYI

### Classification and Reasoning
- Uses structured prompts to classify each email into predefined categories  
- Ensures consistent JSON outputs for downstream processing  
- Includes validation and recovery prompts to handle malformed responses

### Summaries and Reporting
- Generates summaries for:
  - Urgent and high-priority emails  
  - Deadlines and required follow-ups  
  - Key trends and observations  

### LLM-as-Judge Evaluation
- Scores the output against key criteria: Innovation, Approach, Significance, and Expertise  
- Produces justification, strengths, weaknesses, and recommendations  

---

## Technologies Used
- Python  
- OpenAI API  
- Prompt Engineering  
- JSON schema and validation  
- Yesterbox methodology  
- LLM-as-Judge evaluation  
- Jupyter Notebook  

---

## Project Structure

    ai-email-secretary-yesterbox
    │
    ├── JHU_AGAI_W9_Mid_Term_Project_Learners_Notebook_43.ipynb
    ├── README.md
    └── requirements.txt   (optional)

---

## Installation

To clone the repository:

    git clone https://github.com/<your-username>/ai-email-secretary-yesterbox.git
    cd ai-email-secretary-yesterbox

Install dependencies:

    pip install -r requirements.txt

Or manually:

    pip install openai python-dotenv

---

## Running the Notebook

1. Open the notebook in Jupyter, VS Code, or Google Colab  
2. Add your OpenAI API key to your environment  
3. Run the cells in order  
4. Upload an email file using the filename pattern  
5. Review classifications and evaluation output  

### Configuration

Create a `config.json` file in the project directory. This file stores your OpenAI API key and the API base URL.

Use this structure:

```json
{
    "API_KEY": "your_openai_api_key_here",
    "OPENAI_API_BASE": "https://aibe.mygreatlearning.com/openai/v1"
}

---

## Background (Optional)

This project started in a graduate-level generative AI course at Johns Hopkins but has since been expanded with improved prompts, validation logic, and evaluation workflows.

---

## Future Enhancements
- Gradio user interface  
- HuggingFace Space deployment  
- Email inbox integration  
- Vector database for long-term memory  
- Agent-based follow-up actions  

---

## Contact
Feel free to open an issue or reach out with questions.


## **Project Structure**

