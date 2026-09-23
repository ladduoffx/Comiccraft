# Phase 4: Development & Coding

## Development Log:
- Day 1: Created Streamlit app skeleton with title and input box.
- Day 2: Integrated Hugging Face Inference API for Stable Diffusion XL.
- Day 3: Solved character consistency issue using same seed + prompt engineering.
- Day 4: Added dialogue generation using LLM prompt: "Generate funny dialogues for these scenes".
- Day 5: Implemented PDF download feature using ReportLab.
- Day 6: Bug fixing - Image generation failing on long prompts. Added prompt trimming.
- Day 7: UI polishing and deployment ready.

## Challenges Faced:
1.  Character face changing in every panel - Solved by using LoRA and fixed seed.
2.  API rate limits - Added time delay and error handling.
3.  Streamlit session state losing data - Used st.session_state.

## Code Structure:
- app.py: Main Streamlit application
- utils.py: Image generation and PDF functions
- requirements.txt: All dependencies
