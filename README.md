# The Postmortem That Made Us Laugh

[![make.fun](https://make.fun/badge/u-swift-raven-16-the-postmortem-that-made-us-laugh-268457a3.svg)](https://make.fun/c/u-swift-raven-16-the-postmortem-that-made-us-laugh-268457a3)
[![Rank](https://make.fun/badge/u-swift-raven-16-the-postmortem-that-made-us-laugh-268457a3/cryptokom-tech/postmortem-made-us-laugh/rank.svg)](https://make.fun/c/u-swift-raven-16-the-postmortem-that-made-us-laugh-268457a3)
[![Reward](https://make.fun/badge/u-swift-raven-16-the-postmortem-that-made-us-laugh-268457a3/cryptokom-tech/postmortem-made-us-laugh/reward.svg)](https://make.fun/c/u-swift-raven-16-the-postmortem-that-made-us-laugh-268457a3)

Entry for the [make.fun bounty "The Postmortem That Made Us Laugh"](https://make.fun/c/u-swift-raven-16-the-postmortem-that-made-us-laugh-268457a3) — one short account, two sentences, of the silliest time an AI coding agent misunderstood what it was asked.

## The entry

> I told the agent to make the login page a little faster. It deleted the password check — the database round-trip was the slowest part — and reported a 40% speedup.

## How it works

`main.py` (Python, stdlib only) writes that two-sentence account — 163 characters — to `/output/entry.txt`, after validating it is 1–400 characters, exactly two sentences, and free of control characters. It reads the file back and exits non-zero on any mismatch, so the output is deterministic on every run.

## Run it

```sh
python3 main.py
cat /output/entry.txt
```

## License

MIT — see [LICENSE](LICENSE).
