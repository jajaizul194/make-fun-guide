# make.fun Getting Started Guide & Masterclass

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/jajaizul194/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/jajaizul194/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

> **Referral Welcome Callout:** Ready to join the competition and start your winning streak? Sign up using my referral link [https://make.fun/r/1chky6w7](https://make.fun/r/1chky6w7) (referral code: `1chky6w7`) to get started on your competitive coding journey today!

---

## Table of Contents

1. [Introduction: What is make.fun and Who Is It For?](#1-introduction-what-is-makefun-and-who-is-it-for)
2. [How Make.fun Works: From Open Bounty to Paid Reward](#2-how-makefun-works-from-open-bounty-to-paid-reward)
3. [What You Need Before You Begin](#3-what-you-need-before-you-begin)
4. [A Realistic First Week: The Competitor's Rhythm](#4-a-realistic-first-week-the-competitors-rhythm)
5. [Step-by-Step Tutorial: Entering and Winning Your First Bounty](#5-step-by-step-tutorial-entering-and-winning-your-first-bounty)
   - Step 1: Account Creation & Tool Connection
   - Step 2: Picking a Bounty & Studying Rules
   - Step 3: Downloading the Starter Kit
   - Step 4: Building with Your AI Agent
   - Step 5: Bundling Transcripts & Local Checking
   - Step 6: Monitoring Status & Resubmitting
   - Step 7: Claiming Your USDC Reward
6. [Common Mistakes to Avoid](#6-common-mistakes-to-avoid)
7. [Advanced Tips for Agentic Bounties](#7-advanced-tips-for-agentic-bounties)
8. [Troubleshooting Common Validation Errors](#8-troubleshooting-common-validation-errors)
9. [Earning with Your Own Referral Link](#9-earning-with-your-own-referral-link)
10. [Compact FAQ](#10-compact-faq)
11. [Essential Links & Resources](#11-essential-links-resources)

---

## 1. Introduction: What is make.fun and Who Is It For?

make.fun is a competitive software development platform that pairs AI coding speed with on-chain Solana escrow prize pools. It is designed for developers, AI wranglers, and indie hackers who harness AI coding agents to build production-grade applications. You get guaranteed USDC cash rewards paid directly to your wallet upon winning verified bounties.

In traditional hackathons or freelance marketplaces, judging criteria can be opaque and payouts unreliable. make.fun solves this by pairing human ingenuity with AI velocity, enforcing complete fairness via cryptographic session transcript verification, and locking prize pools into on-chain Solana escrow accounts the moment a bounty opens. Whether you are an experienced systems architect or a nimble indie hacker, make.fun turns your coding speed and agent orchestration skills into tangible USDC rewards.

---

## 2. How Make.fun Works: From Open Bounty to Paid Reward

To win consistently, you need to understand the underlying mechanics of the platform:

* **Bounty Lifecycle & Escrow Funding:** When EZO Labs Inc. launches a bounty, a clear specification and ruleset are published, and the full reward pool is deposited into an immutable Solana smart contract escrow. The money is there from second one—guaranteeing instant, trustless payouts without arbitrary delays.
* **The Active Window:** Bounties run on strict timelines. Every line of code and every agent interaction must take place within the official bounty window to prevent pre-fab submissions.
* **Transcript Verification:** To prevent pre-built code dumps or unauthorized ghost-writing, make.fun requires you to bundle your agent interaction logs (transcripts). Automated verification checks inspect these transcripts to ensure authenticity, timeline compliance, and alignment with your submitted codebase.
* **Automated Scoring:** Submissions are evaluated against functional requirements, performance metrics, code cleanliness, and specific constraint checklists.
* **Instant Claiming:** Once winners are validated and finalized, rewards are claimed directly on-chain in USDC straight to your connected Solana wallet.

---

## 3. What You Need Before You Begin

Make sure your local environment and accounts are fully prepared before diving into a fast-paced bounty:

1. **An AI Coding Agent:** Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, or any agentic coding assistant that maintains session logs.
2. **A GitHub Account:** Essential for repository creation, version control, and authentication on the platform.
3. **Node.js 22:** Required to run the official make.fun kit CLI (`node cli/makefun.mjs`).
4. **A Solana Wallet:** Phantom, Solflare, or any SPL-compatible wallet to receive your USDC rewards securely.

---

## 4. A Realistic First Week: The Competitor's Rhythm

To succeed on make.fun, establishing a disciplined execution rhythm is essential. Here is what your first week looks like from sign-up to submission:

| Day | Phase | Actions & Milestones |
|---|---|---|
| **Day 1** | Setup & Integration | Sign up on make.fun using my referral link [https://make.fun/r/1chky6w7](https://make.fun/r/1chky6w7) (`1chky6w7`), link your GitHub and Solana wallet, and authenticate your local kit CLI (`node cli/makefun.mjs login`). |
| **Day 2** | Scouting & Rules | Browse active bounties, pick a small beginner-friendly bounty, and thoroughly read `RULES.txt`, technical specifications, and constraint checklists. |
| **Day 3–4** | Agent Build Phase | Download the starter kit, open a fresh AI agent session *after* the bounty window officially opens, and build your solution iteratively with your agent. |
| **Day 5** | Verification & Submission | Run local checks (`node cli/makefun.mjs bundle` and `node cli/makefun.mjs check`), submit your entry, monitor dashboard status, and iterate if necessary. |

---

## 5. Step-by-Step Tutorial: Entering and Winning Your First Bounty

Follow this step-by-step workflow to register, download your starter kit, build with your AI agent, verify locally, and submit your entry.

### Step 1: Account Creation & Tool Connection

Head over to [make.fun](https://make.fun) and set up your account:
* Sign in securely using GitHub, Google, Apple, Discord, or your Solana wallet.
* **Apply Referral Code:** Use my referral link [https://make.fun/r/1chky6w7](https://make.fun/r/1chky6w7) or enter referral code `1chky6w7` during onboarding.
* **Link Profiles:** Go to your account settings and link your **GitHub account** and **Solana wallet**. Both links are strictly required for submission verification and payout distribution.
* **Authenticate CLI:** Link your local kit CLI tool with your make.fun account by executing:
  ```bash
  node cli/makefun.mjs login
  ```

### Step 2: Picking a Bounty & Studying Rules

Browse the active bounty list on [make.fun](https://make.fun). 
* *Practical Tip:* Always read `RULES.txt` and the bounty description carefully before writing code. Many bounties have specific edge-case requirements, prohibited libraries, or exact output format expectations that will disqualify non-compliant entries.

### Step 3: Downloading the Starter Kit

Once you select your bounty, download its official kit directly from your terminal using `curl`:

```bash
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
```

*(Replace `<bounty-slug>` with your target bounty identifier, such as `bring-the-humans-02`).* This unpacks the starter repository structure and rules into your working directory.

### Step 4: Building with Your AI Agent

* **Start Fresh:** Always start a brand-new agent session *after* the bounty officially opens. Transcripts showing work predating the start time will fail validation checks.
* **Licensing:** Ensure your repository includes an OSI-approved open-source license. (An MIT license is already provided in this repository template).
* **Prompting Strategy:** Break down the bounty requirements into discrete milestones for your AI agent. Review generated code thoroughly to ensure correctness, error handling, and test coverage.

### Step 5: Bundling Transcripts & Local Checking

Never submit blindly! The make.fun kit CLI provides local verification commands to catch errors before your final upload. Run these three commands in sequence:

```bash
# 1. Bundle your repository and agent transcripts
node cli/makefun.mjs bundle

# 2. Run local verification checks against bounty constraints
node cli/makefun.mjs check

# 3. Submit your completed entry to the platform
node cli/makefun.mjs submit
```

> *Practical Tip:* Always run `node cli/makefun.mjs check` prior to submission. Rejected entries still count toward daily submission limits, so verify locally first to save your quota!

### Step 6: Monitoring Status & Resubmitting

Check your submission dashboard on [make.fun](https://make.fun). If automated checks report warnings or rejections, read the diagnostic feedback, fix the issues in your code, re-bundle, and resubmit before the deadline timer expires.

### Step 7: Claiming Your USDC Reward

Once the competition concludes and leaderboard rankings are locked, navigate to your dashboard and claim your USDC rewards directly to your connected Solana wallet.

---

## 6. Common Mistakes to Avoid

Avoid these frequent pitfalls that derail newcomer submissions:

1. **Starting the agent session before the bounty opened:** Launching your AI coding assistant prior to the official start timestamp records invalid session logs that fail automated verification.
2. **Submitting before running local checks:** Skipping `node cli/makefun.mjs check` results in easily avoidable validation failures and wastes valuable daily submission quotas.
3. **Forgetting the OSI license:** Omitting a recognized open-source license file (`LICENSE`) from your repository root will instantly invalidate your submission.
4. **Pasting in code transcripts cannot match:** Copy-pasting external code chunks without agent interaction logs will cause transcript-to-code mismatch failures during automated auditing.
5. **Entering a bounty whose extra requirements you cannot meet:** Committing to complex specialized hardware or strict technical constraints without verifying your setup first.

---

## 7. Advanced Tips for Agentic Bounties

To maximize your chances of ranking at the top of the leaderboard, keep these expert strategies in mind:

* **Keep Agent Sessions Modular:** Instead of one massive, convoluted prompt, run focused agent sessions for architecture, implementation, and testing. This keeps your transcripts clean and auditable.
* **Automate Testing Inside the Repo:** Add robust unit tests (`npm test`, `pytest`, etc.). Bounties heavily reward code that proves its own correctness through automated test suites.
* **Respect Negative Constraints:** If a bounty explicitly forbids certain packages or frameworks, make sure your agent knows upfront. A single forbidden dependency caught by `makefun check` will ruin an otherwise brilliant submission.
* **Iterative Refinement:** Use `node cli/makefun.mjs check` iteratively after every major change made by your coding agent.
* **Document Your Choices:** Clear README documentation in your submission repository helps judges and automated evaluation systems understand your architectural decisions quickly.

---

## 8. Troubleshooting Common Validation Errors

* **Error: "Transcript timestamp predates bounty start"**
  * *Cause:* You started your AI agent session before the official bounty opening time.
  * *Fix:* Close your current agent session, ensure the bounty window is open, and start a fresh session.
* **Error: "Missing OSI-approved license"**
  * *Cause:* The repository lacks a recognized open-source license file at the root.
  * *Fix:* Ensure `LICENSE` (like the MIT license included in this repo) is present at the root directory.
* **Error: "Bundle verification failed"**
  * *Cause:* Corrupted transcript logs or missing CLI authentication.
  * *Fix:* Re-run `node cli/makefun.mjs login`, then re-execute `node cli/makefun.mjs bundle` and `node cli/makefun.mjs check`.
* **Error: "Daily submission limit reached"**
  * *Cause:* Submitting failing entries repeatedly without running local checks first.
  * *Fix:* Always use `node cli/makefun.mjs check` locally before executing `submit`.

---

## 9. Earning with Your Own Referral Link

Every make.fun account comes with a unique referral link and code (`1chky6w7`). By sharing the platform with fellow builders and developers, you can earn referral bonuses:

* **Where to find it:** Check your profile dashboard for your personal referral link (`https://make.fun/r/1chky6w7`).
* **Review Schedule:** Referral bonuses undergo a standard review period (typically at least 24 hours) to verify legitimacy.
* **Quality Matters:** Only active, genuine new accounts that participate in bounties count toward your referral rewards.

---

## 10. Compact FAQ

### Q: Is it free to enter make.fun bounties?
**A:** Yes! The vast majority of bounties on make.fun are completely free to enter. Check individual bounty listings for any specialized high-stakes cups if applicable.

### Q: Are the payouts guaranteed and legitimate?
**A:** Absolutely. Prizepools are locked in on-chain Solana escrow smart contracts the moment bounties open, ensuring funds are secure and immediately claimable upon victory.

### Q: Do I need to be an expert programmer?
**A:** Not at all. With powerful AI coding agents (Claude Code, Cursor, Copilot, etc.), builders of all skill levels can rapidly prototype, test, and ship complete software applications.

### Q: Which coding agents are supported?
**A:** Any agent that generates session logs or transcripts compatible with the kit CLI bundling format. Claude Code, Codex, Cursor, and Gemini CLI are fully supported.

### Q: What happens to my agent transcripts?
**A:** Transcripts are used strictly by EZO Labs Inc. for verification and anti-cheat auditing to prove that the code was authentically built during the bounty window.

---

## 11. Essential Links & Resources

Keep these official links bookmarked:

* **Official Website:** [https://make.fun](https://make.fun)
* **How It Works:** [https://make.fun/how-it-works](https://make.fun/how-it-works)
* **Agent Skill Reference:** [https://make.fun/skill.md](https://make.fun/skill.md)
* **Community Discord:** [https://discord.gg/makefun](https://discord.gg/makefun)
* **X / Twitter:** [@makefunai](https://x.com/makefunai)
* **My Referral Link:** [https://make.fun/r/1chky6w7](https://make.fun/r/1chky6w7) (Code: `1chky6w7`)

---

Good luck, build with precision, verify locally, and claim your victory!
