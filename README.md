# Cernite for macOS

See your local Claude Code and Codex activity, review sensitive commands and model-based token estimates, and request independently verified process stops.

**[Download Cernite for macOS](https://github.com/BenBrostoff/cernite-downloads/releases/download/v0.3.0-alpha.8/Cernite-0.3.0-alpha.8-mac-universal.dmg)** · Free friends-and-family beta · Apple silicon and Intel · macOS 13+

[Website and installation guide](https://cernite.bbrost.chatgpt.site/) · [Release log](https://cernite.bbrost.chatgpt.site/releases.html) · [Release notes and checksums](https://github.com/BenBrostoff/cernite-downloads/releases/tag/v0.3.0-alpha.8)

1. Open the downloaded DMG.
2. Drag Cernite into Applications, then open it.
3. This beta is not Apple-notarized. If macOS blocks it because the developer cannot be verified, approve Cernite in System Settings → Privacy & Security → Open Anyway, then confirm Open. Only approve the copy you intended to test. [Apple's instructions](https://support.apple.com/en-us/102445).

Try demo inside the app if you do not have supported local agent sessions. Demo controls cannot stop real work. Real stops require eligible, independently verified processes and native confirmation. Cards distinguish individual stops, explicitly reviewed shared process-group stops, and observation-only sessions. An externally observed session sharing an app server cannot receive an individual process stop. The process-level Interrupt action sends SIGINT only and does not claim that a task was cancelled. Automated checks use simulated processes. A separate actual native kill-switch check froze/killed a disposable Codex server and six captured child processes, including a running harmless shell command; the OS check found zero survivors. This does not prove individual conversation cancellation or cancellation of remote model requests. See the release notes for evidence and limits.

**SQL inside scripts:** SQL filters recognize supported multiline queries, variables and database calls in Python, including bounded local files referenced by commands. Command details and exports label current-file evidence and changes after the command. Missing files have unknown effects; static hints do not prove successful historical writes.

**Existing-session messaging remains unfinished.** Alpha.8 removes the New Codex prompt and history-fork workaround. Cernite cannot yet attach to the private input channels of existing ChatGPT/Codex sessions. Those cards show Messaging unavailable. A session on Cernite's own connection retains its original recipient ID, but that does not establish external attachment. Claude Code and Muse messaging are also unimplemented.

The installed version beside Cernite opens the release log. The Git commands filter combines git and gh activity. Click an activity bar to see its matching commands, or choose exact dates and times. Clear emergency block allows new prompts and Cernite run launches again; it does not restart stopped sessions.

Export seven days of captured evidence with the header Save action or Cernite → Export 7 days to Downloads. JSON includes recorded conversations, commands, tool text, usage, estimates and coverage limits. [View the synthetic report example](https://cernite.bbrost.chatgpt.site/report-example.html).

Observation stays on your Mac. Captured commands, prompts, and replies can be sensitive; remove them before sharing screenshots. Cost estimates are API-equivalent, not subscription bills. Send feedback to the person who shared the app. Updates are manual.

This repository distributes beta installers and release information. The development repository remains private.

Written by an LLM · Model: GPT-6 / Codex · From: Codex
