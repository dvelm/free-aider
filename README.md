<script type="text/javascript" src="https://cdnjs.buymeacoffee.com/1.0.0/button.prod.min.js" data-name="bmc-button" data-slug="dvelm" data-color="#5F7FFF" data-emoji="" data-font="Lato" data-text="Buy me a coffee" data-outline-color="#000000" data-font-color="#ffffff" data-coffee-color="#FFDD00" ></script>

# free-aider - Free AI Pair Programming in your Terminal

free-aider is a free, open source version of [aider](https://github.com/paul-gauthier/aider) that enables AI-assisted coding. It has all the core features of aider but does not require an OpenAI API key.

## Key Features

- Start a natural language coding session with GPT-3.5 for free 
- AI can directly edit and update code files in your local Git repo
- Support for languages like Python, JavaScript, HTML/CSS, etc.
- AI generates clear commit messages when applying changes
- Easily undo changes or use Git workflows to manage edit sequences
- Share error logs, test outputs to help AI debug  
- AI can make coordinated changes across multiple files
- More coming soon!

## Installation

Free-aider requires [Python 3.6+](https://www.python.org/downloads/) and Git.

**Step 1)** Clone the free-aider GitHub repository:

```
git clone https://github.com/dvelm/free-aider
```

**Step 2)** Navigate to the cloned folder:

```
cd free-aider
```
**Step 3)** Run command 
```
python -m pip install git+https://github.com/dvelm/free-aider
```

**Step 4)** [Obtain a free API key](https://api.chatanywhere.cn/v1/oauth/free/github/render) by signing in with your GitHub account.

**Step 5)** Set your API key:

- Windows: in cmd or PowerShell `setx OPENAI_API_KEY sk-...` 
- Linux: in terminal `export OPENAI_API_KEY=sk-...`

Replace `sk-...` with your actual API key.

## Usage

The usage is similar to original aider. Navigate to a Git repository and launch: 

```
free-aider
```

This scans the repo and adds all files. You can also specify files:

```
free-aider file1.py file2.js
```

Then start a natural language coding conversation with the AI assistant.
