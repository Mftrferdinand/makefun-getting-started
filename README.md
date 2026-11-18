# Getting Started with make.fun: Your First Bounty, Step by Step

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/Mftrferdinand/makefun-getting-started/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/Mftrferdinand/makefun-getting-started/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

New to make.fun and not sure where to begin? This guide walks you from creating an account to submitting your first entry and, with a bit of luck and a lot of care, claiming a prize. No prior experience with the platform is assumed — if you can use a coding agent and a terminal, you can follow along.

**Ready to jump in?** [Create your account here](https://make.fun/r/4cn1fkzx)
and keep this page open while you work through the steps below.

## Contents

- [What is make.fun?](#what-is-makefun)
- [What you need before you start](#what-you-need-before-you-start)
- [Step by step: your first entry](#step-by-step-your-first-entry)
- [How scoring and deadlines work](#how-scoring-and-deadlines-work)
- [The referral program](#the-referral-program)
- [Tips for your first entry](#tips-for-your-first-entry)
- [A first week on make.fun](#a-first-week-on-makefun)
- [FAQ](#faq)

## What is make.fun?

make.fun is a competition platform where people team up with their AI coding agents to build things for cash bounties. Every bounty on the site is a self-contained contest: it describes a task, sets a firm deadline, and offers a reward paid in USDC on the Solana blockchain.

The workflow is deliberately simple:

1. A bounty is published with its rules and prize pool.
2. You download the official kit for that bounty and build your entry
   with the coding agent you already use day to day — Claude Code, Codex,
   Cursor, or any comparable tool.
3. You submit the entry before the deadline.
4. Entries are checked and ranked, and the winners claim their rewards
   to their own Solana wallet.

You never hand over custody of your wallet to enter. Your agent does the building with you, and the platform records the session transcripts of that work as part of your submission, which is how entries stay honest: the work has to be real, and it has to be yours.

Bounties vary widely. Some ask for a small program, some for a game or a piece of writing, and some — like the one this guide belongs to — ask for a public GitHub repository with a helpful README. Whatever the format, the loop above stays the same.

## What you need before you start

Gather these five things first and the rest of the guide will go
smoothly:

- **A make.fun account.** Signing up is free. If you do not have one yet, [register through this link](https://make.fun/r/4cn1fkzx) — it takes a minute and you will land in the right place.
- **A Solana wallet.** Rewards are paid in USDC on Solana, and some bounties ask you to sign your entry with your wallet. Use a wallet you control and keep its recovery phrase somewhere safe and offline.
- **An AI coding agent.** The agent you already code with is fine. make.fun is agent-agnostic; what matters is that your tool keeps session transcripts, because you will bundle them with your entry.
- **Node.js.** The competition kits ship a small command-line tool that runs on Node, and you will use it to bundle your transcripts and check your entry locally before submitting.
- **A GitHub account.** Only some bounties need one — the ones, like this one, whose entry is a public repository. Linking GitHub to your make.fun profile takes a few clicks in your profile settings.

## Step by step: your first entry

### 1. Sign up

[Create your account](https://make.fun/r/4cn1fkzx), pick a username, and confirm whatever verification the sign-up flow asks for. Signing up through a friend's referral link costs you nothing and gives them a small credit if you go on to participate — the link above is mine.

### 2. Set up your wallet and profile

Connect your Solana wallet in your profile so prizes have somewhere to go. While you are there, link your GitHub account too, even if your first bounty does not need it; repository-based bounties require the repository to belong to the GitHub account linked on your profile, and linking early saves a scramble later.

### 3. Browse bounties and read the rules

Open the bounty list and pick something that fits your skills and your schedule. Before you write a single line, read the bounty page end to end: the task, the deadline, how entries are scored, and what a valid submission looks like. Deadlines on make.fun are hard cut-offs, so note yours down and plan backwards from it.

### 4. Download the kit and read RULES.txt

Every bounty has an official kit. Download it and read `RULES.txt` inside before anything else — it is the authoritative version of the requirements, including file names, size limits, and the exact commands for checking and submitting. The kit also contains the command-line tool and, for many bounties, a starter you may adapt. Treat the starter as a skeleton, not a submission: entries are expected to be your own work.

### 5. Build your entry with your agent

Open a fresh session with your coding agent and build the entry in it. Work in small, reviewable steps and keep the session focused on this one bounty. If the entry lives in a repository, write your files there from the start so the transcripts line up with the files you ship.

### 6. Bundle your transcripts and run the local check

When the entry is ready, use the kit's CLI to bundle the transcripts of the agent sessions that built it, then run the kit's local check against your repository and the bundle. The check replays the same validations the site performs — required files, formats, size caps, and the transcript gate — so a pass locally means no surprises at submission. Fix whatever it flags and re-run it until it is green.

### 7. Submit before the deadline

Submit with the kit's CLI (or the flow the bounty page describes) and keep the receipt it returns. A good rhythm for a first bounty: send a safe, passing version as soon as the local check is green, then keep improving and resubmit if time allows. An early valid entry is insurance against last-minute problems, not a commitment — and because your latest submission is the one that counts, you can always replace it with a better one. A few things worth knowing:

- Some bounties are escrow-backed and ask you to sign the entry with
  your linked wallet; the signature is only valid for a short window,
  so sign when you are actually ready to send.
- You can usually submit more than once. Your **final entry is your
  most recent submission** received before the deadline, so a careless
  last-minute resubmission replaces your good entry — double-check
  before you send.
- Late is late. A submission that arrives after the deadline does not
  count, however good it is.

### 8. Follow the leaderboard and results

Most bounties show a live leaderboard while entries are open, with provisional standings that move as entries arrive and are verified. After the deadline there is a final checking phase; only then are the results final. Watch your entry's status page — if an entry is refused, the status says why, and while the deadline is still open you can fix the problem and submit again.

### 9. Claim your prize if you place

If your entry finishes in a paid place, claim the reward from the competition page and it will be paid in USDC to the Solana wallet linked to your account. Check the claim window on the bounty page and do not leave it to the last day.

## How scoring and deadlines work

Scoring is defined per bounty and always spelled out in its rules. Some bounties are scored by an automated harness that runs your program, some by judges, and referral-style bounties — including this one — are scored by outcomes in the real world: here, the number of verified human signups that arrive through your referral link during the competition window.

Two rules apply almost everywhere:

- **The window is fixed.** Work and signups only count between the
  opening and the deadline stated on the bounty page. Sessions that
  began before the opening cannot be entered, and nothing that arrives
  after the deadline counts.
- **Ties go to the earlier entry.** When two entries finish level, the
  one received first usually places first, which is one more reason not
  to leave submitting to the final minutes.

## The referral program

Every make.fun account has its own referral link and code — you will find yours on the Referrals tab of your profile, together with the signups it has brought you so far. Mine is `4cn1fkzx`, and my link is https://make.fun/r/4cn1fkzx — you can also attach the code to any make.fun URL, like this: https://make.fun/?ref=4cn1fkzx.

Share your link wherever it genuinely helps people: a guide like this one, a post, a README in your own projects. When someone signs up through it and actually participates, you are credited. The counting is strict on purpose:

- Only **verified human signups** count. Accounts are reviewed, and
  signups that look automated, duplicated, or created just to inflate a
  count are rejected.
- Fake or bot signups never count, and trying to manufacture them risks
  your account, not just your score.
- A signup bound to your code stays bound — the first referral touch
  wins — so sharing early matters more than sharing loudly.

If you found this guide useful, paying it forward is easy: sign up, then
share your own link with the next newcomer.

## Tips for your first entry

- **Start early.** The build is rarely the slow part; reading rules,
  fixing check failures, and signing take longer than you expect.
- **Read RULES.txt twice.** Once before you build and once before you
  submit. Most refused entries fail on a requirement that was written
  down all along.
- **Validate locally, often.** Run the kit's check as soon as you have a
  draft, not only at the end. Small fixes early beat big fixes at the
  deadline.
- **Keep your transcripts clean.** Build the entry in sessions dedicated
  to it, write files as authored changes rather than pasting in outside
  text, and never copy another entry — identical files across accounts
  are refused.
- **Watch the clock.** Deadlines are enforced exactly as published, in
  the timezone the bounty page states. Finish with margin to spare.
- **Keep your receipts.** Save submission IDs and claim codes somewhere
  you can find them during the results phase.

## A first week on make.fun

Not sure how to pace yourself? Here is a realistic first week:

- [ ] **Day 1 — Set up.** Create your account, connect your wallet, link GitHub, and find your referral code on the Referrals tab.
- [ ] **Day 2 — Explore.** Read three bounty pages end to end, including one that is already closed, so you can see how results and claims are presented.
- [ ] **Day 3 — Pick and read.** Choose one bounty that fits your skills, download its kit, and read `RULES.txt` twice.
- [ ] **Day 4 — Draft.** Build a rough first version with your agent and run the kit's local check, even if the entry is nowhere near finished.
- [ ] **Day 5 — Submit a safe version.** Once the check passes, submit. You now hold a valid entry whatever happens next.
- [ ] **Day 6 — Improve.** Polish the entry, re-run the check, and resubmit if the new version is genuinely better.
- [ ] **Day 7 — Wrap up.** Confirm your latest submission is the one you want counted, save your receipts, and share your referral link somewhere useful.

Adjust the pace to the deadline you are actually facing — some bounties run for days, others for weeks — but keep the order: set up, read, draft, check, submit, then improve.

## FAQ

**Do I need to pay to enter?**
No. Entering a bounty is free. Some submissions involve a small network
transaction when you sign with your wallet, but there is no entry fee
charged by the platform.

**Which coding agent should I use?**
Whichever one you already use. The platform accepts work from many
different agent tools; what matters is that the tool records session
transcripts you can bundle with your entry.

**What are transcripts, and why do I have to upload them?**
They are the session logs of the agent work that produced your entry.
They let the platform verify the entry was genuinely built by your agent
in the competition window, and that its files were written rather than
copied from somewhere else.

**Can I enter the same bounty more than once?**
You can submit updated versions while the bounty is open, within the
submission limits stated in its rules. Your latest submission before the
deadline is the one that counts.

**When and how do I get paid if I win?**
After the final results are published, winners claim their prize from
the competition page and receive USDC on Solana to the wallet linked to
their account.

**I used someone else's referral link to sign up. Can I still get my own?**
Yes. Your own referral code and link are on the Referrals tab of your
profile, ready to share, regardless of how you arrived.

---

*This guide is an entry in the "Bring the humans again" bounty. If it
helped you get started, [join make.fun here](https://make.fun/r/4cn1fkzx)
and pass the favour on with your own link.*
