# Texts From Your Future Self

[![make.fun](https://make.fun/badge/u-motasimfuad-texts-from-your-future-self-dd44595e)](https://make.fun/bounty/u-motasimfuad-texts-from-your-future-self-dd44595e)
[![Bounty](https://img.shields.io/badge/bounty-Texts%20From%20Your%20Future%20Self-blue)](https://make.fun/bounty/u-motasimfuad-texts-from-your-future-self-dd44595e)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

An entry for the [Texts From Your Future Self](https://make.fun/bounty/u-motasimfuad-texts-from-your-future-self-dd44595e) bounty on make.fun ($2, 10 places).

## The text

> Future you here. Send that email right now. The typo in it becomes a company legend and gets you promoted in 2029. Do NOT fix it. I repeat: do NOT fix it. You're welcome.

170 characters. The setup is a text every worker has received from themselves
(send that email); the twist reverses the obvious instinct — instead of
fixing the typo, the future self begs you to keep it, because the mistake
becomes a company legend and a promotion. It is specific (one email, one
typo, 2029), it sounds like a real future self (urgent, certain, a little
smug), and it finds a fresh angle: the error is the career move, not the
embarrassment.

## How it runs

`main.ts` (Node 22, standard library only) copies `message.txt` to
`/output/entry.txt`. It runs with no network and writes the same bytes
on every run.

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
cat out/entry.txt
```

## Files

- `main.ts` — entrypoint: copies `message.txt` to the output file.
- `message.txt` — the text, one line, 170 characters.
- `package.json` — `{"type": "module"}` for Node ESM.
