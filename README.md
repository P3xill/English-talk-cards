# English Talk Cards

A simple tool for English teachers to help students practice speaking.

## What is this?

A website that shows speaking prompts one at a time. Students talk about the topic shown, and when they're done, the teacher clicks to show a new random question.

## How to Start

### On Mac

1. Open the **Terminal** app (search for "Terminal" in Spotlight)
2. Copy and paste this command, then press Enter:

```
cd ~/Desktop/English-talk-cards && python3 -m http.server 8000
```

3. Open your web browser and go to: **http://localhost:8000**

### On Windows

1. Open **Command Prompt** (search for "cmd" in the Start menu)
2. Copy and paste this command, then press Enter:

```
cd Desktop\English-talk-cards && python3 -m http.server 8000
```

3. Open your web browser and go to: **http://localhost:8000**

## How to Use

- **Click the question box** or the **Next →** button to show a new random question
- **Click ← Back** to return to the previous question
- **Keyboard shortcuts**: Use arrow keys (← →), Space, or Enter to navigate

## How to Stop

When you're done, close the Terminal/Command Prompt window, or press `Ctrl + C` in the terminal.

## Changing the Questions

To use your own questions:

1. Open the file `english_speaking_questions_1000.txt` with any text editor
2. Write one question per line
3. Save the file
4. Refresh the browser page

## Troubleshooting

**"Command not found" error?**
Make sure Python is installed on your computer. On Mac, it's usually pre-installed. On Windows, download it from python.org.

**Page won't load?**
Make sure the terminal window is still open and running. Try the steps again from the beginning.
