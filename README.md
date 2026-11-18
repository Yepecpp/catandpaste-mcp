# Cat & Paste connector

Paste a how-to video link. Get a playbook your AI assistant follows when you ask it for advice.

[Cat & Paste](https://catandpaste.app) reads what is said in a public video on YouTube, TikTok, Instagram or Facebook and writes a playbook: the video's method, its steps, numbers and rules, written as instructions an AI assistant follows. The connector puts your playbooks inside your own assistant's chat.

## Add it to your assistant

Connector address:

```
https://api.catandpaste.app/mcp
```

Claude, ChatGPT, Perplexity and Grok accept it as a custom connector. You sign in with your Cat & Paste email and allow access; no key to copy. Step-by-step guides for each assistant: https://catandpaste.app/en/connect

## What it can do

| Tool | What it does | Changes anything? |
|---|---|---|
| Learn a video (`learn_video`) | Sends a public video to the cat, which writes a playbook from it in about two minutes | Yes: starts a read and uses one of your reads |
| List my playbooks (`list_playbooks`) | Shows the title, a one-line description and the platform of each of your playbooks | No, read only |
| Get a playbook (`get_playbook`) | Gives your assistant one playbook in full, to follow in the conversation | No, read only |
| My reads and plan (`get_plan`) | Tells your assistant how many reads you have left, whether a plan renews them each month and when, and whether extra reads are allowed when the month runs out | No, read only |
| Email me the settings link (`email_plan_link`) | When you ask, emails your own account's address a one-use link (60 minutes) to the page where you decide about extras; at most 3 a day | Sends an email; it changes nothing you pay. Only you, signed in, can |

Your assistant sees your playbooks and whether a read started. It never sees your email address, your payments, the video's transcript (the cat never keeps it) or anyone else's playbooks. Disconnect from **Connect your AI** in the app, or in your assistant's settings.

## Things to say

- Learn this video with Cat & Paste: [video link]
- Which Cat & Paste playbooks do I have?
- Use my playbook on Facebook ads to plan this month's budget.
- What does my playbook say I should avoid?
- Which of my playbooks fits what I am working on?

## Teach your assistant

[`skills/cat-and-paste/SKILL.md`](skills/cat-and-paste/SKILL.md) is a small guide that tells an assistant when to reach for your playbooks and how to follow them: check the connector is there, list and read the playbook that fits, learn a shared video link, and report your reads without ever selling.

- Claude, ChatGPT, Gemini and Perplexity: add it from the buttons on [catandpaste.app/en/connect](https://catandpaste.app/en/connect), which download the file each one asks for and show its steps.
- Coding agents (Claude Code, Codex, Cursor and others):

  ```
  npx skills add Yepecpp/catandpaste-mcp --skill cat-and-paste
  ```

## A free playbook

[`playbooks/price-a-service-job/SKILL.md`](playbooks/price-a-service-job/SKILL.md) is a complete example, written from an invented lesson. Playbooks are standard files: Claude, ChatGPT, Gemini and Perplexity accept them as uploads, and any assistant can take the text.

## Listing

[`server.json`](server.json) is the entry in the official registry, `app.catandpaste/catandpaste`.

## Help

hello@catandpaste.app · https://catandpaste.app/en/support · [Privacy](https://catandpaste.app/en/legal/privacy) · [Terms](https://catandpaste.app/en/legal/terms)

The first read is free. Cat & Paste is made by Laye Labs, S.R.L.
