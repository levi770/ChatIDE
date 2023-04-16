<p align="center">
  <a href="https://chatide.dev">
    <img src="https://user-images.githubusercontent.com/3611042/232336469-dfb39213-00b4-48cf-8e4b-c84c111ef30a.png" alt="ChatIDE logo" width="400px">
  </a>
</p>

<p align="center">
    <b>ChatIDE - AI assistant in your IDE</b><br/>
  Converse with <a href="https://openai.com/blog/openai-api" target="_blank">OpenAI's ChatGPT</a> or <a href="https://console.anthropic.com/docs/api" target="_blank">Anthropic's Claude</a> in VSCode
</p>
<p align="center">
<a href="https://marketplace.visualstudio.com/items?itemName=ChatIDE.chatide">
  <img width="309" alt="image" src="https://user-images.githubusercontent.com/3611042/232336724-71df6bf8-94e0-4b08-93fc-089ed70ad8ed.png">
</a>
</p>

<p align="center">
  <a href="https://github.com/yagil/ChatIDE" target="_blank">
      <img src="https://img.shields.io/github/stars/yagil/ChatIDE?style=social" alt="Github repo stars">
  </a>
  <a href="https://github.com/yagil/ChatIDE/blob/main/LICENSE" target="_blank">
      <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="License">
  </a>
</p>

<p align="center">
  <img width="1024" alt="image" src="https://user-images.githubusercontent.com/3611042/232337055-e7800e35-a1b3-4317-8527-b49d0cba0d61.png">
</p>

## Installation

Grab the latest ChatIDE version from the Extensions Marketplace:<br>
https://marketplace.visualstudio.com/items?itemName=ChatIDE.chatide

## Bring Your Own API keys

To use ChatGPT / Claude in ChatIDE, you need to procure API Keys from OpenAI / Anthropic.
- **OpenAI**: https://openai.com/product#made-for-developers
- **Anthropic**: https://console.anthropic.com/docs/api

## Usage

1. Bring up ChatIDE with `Cmd + Shift + i` (or `Ctrl + Shift + i` on non-Apple platforms).
2. Choose your AI model. Currently supported: 
    - `'gpt-4'`,  `'gpt-3.5-turbo'`  (OpenAI)
    - `'claude-v1.3'` (Anthropic)
4. On first usage, you'll be prompted to enter your API key for your chosen AI providers (will be stored in VSCode `secretStorage`).
5. Enjoy!

## Configuration

- Use the `Cmd + Shift + P` keychord and type `>Open ChatIDE Settings`
  - Choose your preferred `model`, `max_tokens`, and `temperature`.
  - Adjust the system prompt to your liking
  - Note: settings will auto save
- Run ChatIDE with `Cmd + Shift + i`. You'll be asked for your OpenAI / Anthropic API key on first time you use the model.
  - Note: your API keys will be stored in [VS Code's `secretStorage`](https://code.visualstudio.com/api/references/vscode-api#SecretStorage)
<p align="center">
  <img width="891" alt="image" src="https://user-images.githubusercontent.com/3611042/232337392-71867aa4-17fc-4328-892e-7a2fff1d5bce.png">
</p>

### Updating your API key

1. Run `cmd + shift + P` (or `ctrl + shift + P`)
2. Start typing `>ChatIDE`

#### OpenAI
3. Select `>Update your OpenAI API Key for ChatIDE`.

#### Anthropic
3. Select `>Update your Anthropic API Key for ChatIDE`.

## Known issues

1. There's currently no way to stop the model from generating. You need to wait until it's done.
2. Closing the ChatIDE pane while the model is generating might lead to a non-recoverable error. You'll need to restart VS Code to use ChatIDE again.
3. Closing / re-opening the ChatIDE pane does not reset the messages history. You can reset the message history by clicking the "Reset Chat" button (don't do this while the model is generating!)

## Warning

⚠️ This is an early prototype, use at your own peril.

🧐 Remember to keep an eye on your OpenAI / Anthropic billing.

## Credits

ChatIDE continues to be built using ChatIDE.
