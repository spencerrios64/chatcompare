# chatcompare

Ask several AIs the same question at once and read the answers side by side.

**Use it here: https://spencerrios64.github.io/chatcompare/**

Supports ChatGPT (OpenAI), Claude (Anthropic), Gemini (Google), Groq, OpenRouter and
DeepSeek. It is a single web page (`index.html`): no server, no install, no dependencies.

## Use

1. Open **Settings**, paste an API key for each AI you want, press **Load models** and pick
   a model. Gemini, Groq and OpenRouter offer free keys; OpenAI and Anthropic charge your
   account per message.
2. Tick the AIs to ask, type one question and press **Ask all**.
3. Read the answers next to each other, with the time and length of each.
4. Optional: pick one AI and press **List the differences**. It reads all the answers and
   lists where they agree, where they differ and what only one of them said.

If you already saved keys in [chatrelay](https://github.com/spencerrios64/chatrelay) in the
same browser, they are copied over the first time, because both pages live on the same site.

## Good to know

- It uses official API keys. It cannot use your normal chatgpt.com or claude.ai login.
- Each question costs one message on every ticked AI, and the comparison costs one more.
- The comparison is written by an AI, so it can be wrong or favour its own answer.
- Each question is sent on its own, with no earlier conversation. Answers are plain text
  and arrive all at once.
- Keys are stored in this browser only (local storage) and are sent only to that AI's own
  API. Anyone who can use your browser profile can read them; use **Forget all keys** on a
  shared computer.
- Tested with simulated API responses. Calls against the real APIs have not been tested
  with live keys yet, and a provider may block direct browser calls.

## Claude plugin

This repo is also a Claude plugin marketplace, so Claude can do the same job in a chat. In Claude Code:

```
/plugin marketplace add spencerrios64/chatcompare
/plugin install chatcompare@chatcompare
```

In the Claude app, download the `plugin` folder as a zip, rename it to `.plugin` and open it in a chat. Details: [plugin/README.md](plugin/README.md).

Part of a family of small tools for AI chats: [chatvault](https://github.com/spencerrios64/chatvault), [chatzip](https://github.com/spencerrios64/chatzip), [chatrelay](https://github.com/spencerrios64/chatrelay), [chatbrief](https://github.com/spencerrios64/chatbrief), [chatscrub](https://github.com/spencerrios64/chatscrub), [chatcompare](https://github.com/spencerrios64/chatcompare), [chatstats](https://github.com/spencerrios64/chatstats) and [promptbank](https://github.com/spencerrios64/promptbank).
