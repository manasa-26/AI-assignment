# AI-assignment
# Meeting Action Item Extractor

##  Project Overview

This project extracts **action items** from meeting transcripts using a Large Language Model (LLM) via the **LangChain** framework and **OpenAI's GPT-4**.

The model reads natural conversation and outputs only the important tasks or decisions discussed.

---

## Tech Stack

- **Python**
- **Google Colab**
- **OpenAI API (GPT-4)**
- **LangChain** – for prompt management and chaining
- **LangChain Community** – for model integration (`ChatOpenAI`)

---

##  Code Explanation

1. **Transcript Input**  
   A sample meeting transcript is provided as a multi-line string.

2. **Prompt Creation**  
   A structured prompt is defined using `ChatPromptTemplate` to tell the model:  
   _“You are an assistant that extracts clear, actionable items…”_

3. **Model Setup**  
   GPT-4 is initialized using `ChatOpenAI` with temperature 0 for deterministic output.

4. **LangChain Chain**  
   The `LLMChain` object connects the prompt and model, allowing the transcript to be passed and processed in one step.

5. **Result**  
   The chain returns a cleaned list of action items, extracted from the meeting discussion.

---

