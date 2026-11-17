<p align="center"><img src="https://looksie.dev/img/icon.png" width="96" alt="Looksie"></p>

# Looksie

**Have a proper looksie at big pull requests.** Looksie is a desktop app for Windows and Mac that turns a big pull
request (the kind coding agents write) into a handful of decisions, walks you through them one at a time, and posts
your review.

**[Download the latest version](https://github.com/marcus-smallman-lewis/looksie-releases/releases/latest)** ·
[Website](https://looksie.dev) · [How it decides](https://looksie.dev/how.html) ·
[Privacy](https://looksie.dev/privacy.html) · [Source code](https://github.com/marcus-smallman-lewis/looksie-open)

Free for public repositories, for good. Private repositories need Pro, with a free trial.

<p align="center"><img src="https://looksie.dev/img/briefing.png" width="720" alt="The briefing: what the change is for, the author's claims checked against the code and CI, and what needs you."></p>

## How it works

1. **Open a pull request.** Looksie lists the ones waiting on you (it uses the GitHub CLI's sign-in, or a token you
   add). Paste `owner/repo#123` to open any other.
2. **Read the briefing.** What the change is for, in the author's words, with each claim ("tests pass", "no breaking
   changes") checked against the code and the CI results.
3. **Make the decisions.** The change is split into steps and read in order: data, server, screens, tests. Only the
   few that need your judgement ask a question, and each says why. Answer Fine, Needs changing or Question, and
   comment on any line. The rest are quick looks.
4. **Send your review.** You see exactly what will be posted, then press Submit. Looksie never comments by itself.

Also: [benchmarks on real pull requests](https://looksie.dev/benchmarks.html).

## Review inside Claude Code or Codex

Connect your own Claude Code or Codex once (Settings, Your AI, Connect). Then, in Claude Code, type
`/looksie:review` (in Codex, `$looksie`), or just ask it to review a pull request. It picks up the one open in
Looksie and goes through the decisions with you in chat. To post, it shows you a preview of exactly what will be sent
and waits for your yes; Claude Code also asks you to approve every post. Answers made in chat show up in the app, and
the other way round.

## Installing

Looksie is not signed by Apple or Microsoft yet, so the first time you open it your computer will ask if you are sure. You only do this once: updates install without asking again.

**Windows:** run `Looksie-windows-setup.exe`. If SmartScreen says it protected your PC, click **More info**, then **Run anyway**.

**Mac:** use `Looksie-mac-apple-silicon.dmg` for a Mac with an Apple chip (M1 and later), or `Looksie-mac-intel.dmg` for an
older Intel Mac (Apple menu → About This Mac says which). Open the .dmg and drag Looksie into Applications. Open it once,
press Done at the warning, then go to **System Settings → Privacy & Security** and click **Open Anyway**.

If the Mac says the app is damaged, run this in Terminal, then open it again:

    xattr -dr com.apple.quarantine /Applications/Looksie.app

After that, Looksie keeps itself up to date: it checks when it opens and every few hours, and installs a new version when you say.

## Questions

Questions, a pull request Looksie got wrong, or a security report: [support@looksie.dev](mailto:support@looksie.dev).
This repository holds the downloads and the website; the code that talks to GitHub, to your AI and to the network is
in [looksie-open](https://github.com/marcus-smallman-lewis/looksie-open).
