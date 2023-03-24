# ChatGPT Commit Assistant

ChatGPT Commit Assistant is a command line tool that generates commit messages for uncommitted changes in a git repository using OpenAI's GPT model.

## Installation

You can install the ChatGPT Commit Assistant using pip: `pip install chatgpt-commit-assistant`

## Usage

After installation, you can use the command `chatgpt-commit-assistant` in your terminal from anywhere within a git repository. The script will generate a commit message for the uncommitted changes in the repository.

It will look for `OPENAI_API_KEY` in your environment variables. You can create keys at https://platform.openai.com/account/api-keys.

For example:

```
$ cd my-git-repo
$ chatgpt-commit-assistant
Generated commit message: Update example feature
Do you approve this commit message? (yes/no):
```

You can then respond with "yes" or "no". If you respond with "no", the script will generate a new commit message and ask for approval again. If you want to exit the script, you can press Ctrl+C.

## Limitations

Right now, this script only works for modifications to pre-existing files. It does not work for untracked files.
