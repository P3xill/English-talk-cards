# English Talk Cards

A browser-based speaking prompt tool for English teachers. It includes a built-in
question bank, manual and timed sessions, and optional Google sign-in for saving
custom questions and projects.

## Use the published app

The GitHub Pages site is:

https://p3xill.github.io/English-talk-cards/

Click the question card or **Next** to generate another question. **Back** returns
to the previous question, and **Start Session** starts the classroom timer.

## Run locally

This is a static site with no build step. From the project directory, run:

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000/. Opening `index.html` directly will not work
reliably because the browser must fetch `questions.txt` over HTTP.

## Publish

GitHub Pages is configured to publish the root of the `main` branch. Pushing a
verified change to `main` triggers the existing Pages deployment; no package
installation or build command is required.

The app's optional sign-in and saved-question features use the existing Firebase
project `english-talk-cards`. For Google sign-in to work on another hostname, add
that hostname to **Firebase Authentication → Settings → Authorized domains**.
Firestore must also keep per-user rules that allow authenticated users to access
only their own questions and projects.

## Content files

- `questions.txt` is the question bank loaded by the app.
- `english_speaking_questions_1000.txt` is an additional source list and is not
  loaded automatically.
