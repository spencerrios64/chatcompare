# chatcompare plugin

Compare answers from several AIs to the same question: where they agree, where they differ, and what only one said.

## What you can ask

- "Help me ask ChatGPT and Gemini the same question" (Claude writes the question to paste)
- "Compare these answers" (paste what each AI said, labelled)
- "Which of these two answers is wrong, and why?"

## What it can't do

A plugin inside Claude cannot call other AIs. You paste the question into each AI and paste the answers back. For one question sent to many AIs automatically, with your own API keys, use the chatcompare web app: https://spencerrios64.github.io/chatcompare/

Project: https://github.com/spencerrios64/chatcompare

## Install

In Claude Code:

```
/plugin marketplace add spencerrios64/chatcompare
/plugin install chatcompare@chatcompare
```

In the Claude app, download the `plugin` folder as a zip, rename it to `.plugin` and open it in a chat.
