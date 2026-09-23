# Phase 3: System Design & Architecture

## System Architecture:
User -> [Streamlit Frontend UI] -> [Python Backend Logic] -> [AI Model APIs] -> [Comic Panels]

## Architecture Diagram (Text):
+---------------+
| User Prompt   |
+-------+-------+
        |
        v
+---------------+       +---------------------+
| Prompt Parser | ----> | Character Consistency |
| (LLM)         |       | Module              |
+-------+-------+       +----------+----------+
        |                          |
        +------------+-------------+
                     |
                     v
          +--------------------+
          | Image Generation   |
          | (SDXL Model)       |
          +---------+----------+
                    |
                    v
          +--------------------+
          | Dialogue & Bubble  |
          | Generator          |
          +--------------------+
                    |
                    v
          +--------------------+
          | PDF / Image Export |
          +--------------------+

## UI Design (Wireframe):
- Title: ComicCraft
- Textbox: Enter your comic story
- Dropdown: Select Art Style [Marvel, Manga, Anime]
- Button: Generate Comic
- Gallery: Display 6 panels with edit option
- Button: Download as PDF

## Database Design:
No database needed for MVP. Session state used.

## Technology Choices:
- Streamlit for fast UI
- Stable Diffusion for image generation
- Groq / OpenAI API for story and dialogue
