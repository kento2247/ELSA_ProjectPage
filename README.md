# ELSA Project Page

This is the project page for the paper **"ELSA: Acoustic Event-Level Semantic Alignment for Fine-Grained Reference-Free Text-to-Audio Evaluation"**.

## Features
- **Bulma Utilities**: Includes Bulma CSS for utility classes while keeping the custom visual theme.
- **Elsa / Frozen Theme**: Deep midnight blue background, icy glassmorphism effects, and animated snow accumulation.
- **Interactive Methodology Pipeline**: A dynamic visualization of the evaluation process (Text → LLM → Audio → LASS → Score).
- **JSON-Driven Demo**: Easily extensible demo section powered by `demo.json`.
- **Carousel Results**: Experimental results and analysis presented in auto-playing carousels.
- **Responsive Design**: Fully optimized for desktop and mobile viewing.

## File Structure
- `index.html`: Main entry point.
- `style.css`: Custom styles (Glassmorphism, Animations, Responsive).
- `demo.json`: Data source for the interactive demo pipeline.
- `statics/`:
    - `images/`: Project assets.
    - `audio/`: Audio samples (place your WAV files here).

## How to Add Demo Samples
1.  Add your audio files to `statics/audio/`.
2.  Open `demo.json`.
3.  Add a new object to the array:
    ```json
    {
      "id": "new_sample",
      "label": "My New Sample",
      "text": "Description of the sample.",
      "parsed": "[\"keyword1\", \"keyword2\"]",
      "audioGen": "statics/audio/my_audio_gen.wav",
      "audioSep": "statics/audio/my_audio_sep.wav",
      "score": "0.95"
    }
    ```
4.  The new sample will automatically appear in the dropdown menu.

## Deployment
Since the demo fetches data from `demo.json`, this page **must be served via a web server** to avoid CORS errors (browsers block `fetch` from local file paths).
- **GitHub Pages**: Simply push to main or gh-pages branch.
- **Local**: Use `python3 -m http.server` or VS Code's "Live Server" extension.

## Setup & Editing

1.  **Content**: Open `index.html` and replace the placeholder text (Abstract, Method descriptions) with the actual content from your paper.
2.  **Audio Samples**: Place your `.wav` or `.mp3` files in `statics/audio/` (create the folder if it doesn't exist) and update the `src` attributes in the `<audio>` tags in `index.html`.
3.  **Authors**: Update the author names and affiliations in the header section.
4.  **Links**: Update the "Paper", "Code", and "Demo" links in the header to point to the actual resources.

## Deployment to GitHub Pages

1.  Push this repository to GitHub.
2.  Go to **Settings** > **Pages**.
3.  Under **Source**, select `Deploy from a branch`.
4.  Select your main branch (e.g., `main` or `master`) and the root folder `/` (or `/docs` if you move files there).
5.  Click **Save**. Your site will be live at `https://<username>.github.io/<repo-name>/`.

## Assets
Images are located in `statics/images/`. ensure you do not move them without updating the references in `index.html`.
