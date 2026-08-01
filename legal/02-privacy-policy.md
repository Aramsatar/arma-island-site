# Privacy Policy — ARMA Island

**Last updated:** [DATE] · **Applies to:** ARMA Island 1.0.1 and later

> **What changed, and why you should trust this version more than the last one.**
> Until 1.0.1 this page said the app had "no networking code in it at all." That
> was not true: it fetched album artwork over HTTPS from your music service. The
> app has been changed rather than the wording — 1.0.1 has no network permission
> at all, so macOS itself refuses any outbound connection. If you are running
> 1.0.0, update.

## The short version

The app sends us nothing, because it cannot. There is no server, no account, no
analytics, no telemetry and no crash reporting. Everything it reads stays on
your Mac.

That is not a promise about our intentions. ARMA Island 1.0.1 ships **without
the `com.apple.security.network.client` entitlement**, which means macOS blocks
outbound connections at the kernel whether or not the code asks for one. You can
check: run it and look at its open sockets. There are none.

**But it reads a lot on your Mac, and you should know exactly what.**

## What it reads, and where that stays

**Your clipboard — continuously, and on by default.** Every 0.7 seconds while
you are active, ARMA Island checks whether you copied something, and keeps a
history so you can paste it back later. Text is stored **in plain text** in a
file on your Mac at `~/Library/Application Support/ARMA Island/`, readable only
by your user account (`0600`), capped at 50 items.

It deliberately refuses to record: anything a password manager marks as
concealed; copies from a list of known password managers; anything oversized;
and — the rule that matters most — **anything that looks like a credential,
whoever it came from**, because a password copied out of a terminal or a `.env`
file arrives unmarked. Those are masked, held in memory so you can still paste
them, and never written to disk.

**There is no automatic expiry.** Items stay until they fall off the 50-item cap
or you clear them. You can clear the history, and you can turn the whole feature
off, in Settings.

**Coding-agent sessions.** It reads session files that Claude Code writes on your
disk, to show what your agents are doing. These contain **the beginning of your
prompts (about 400 characters), the tools the agent ran, the file paths it
touched and the shell commands it executed.** They are deleted when the agent
ends its session, or cleared after 8 hours of staleness.

**It also modifies `~/.claude/settings.json`** to install six hooks, and writes
two small executables it uses to receive those events. It changes another tool's
configuration; you should know that before installing.

**What you are playing.** Asked of Spotify, Music or Chrome over Apple Events.
For Chrome this means the app can see **your window and tab titles** while
looking for a playing tab. macOS asks your permission for this the first time,
and you can refuse it — the app still works, with less.

**Running apps, and sleep/wake.** To know when to hide itself.

All of it stays on your machine.

## Her voice

When you call her with ⌥⌘I she speaks. That is macOS speech synthesis, using a
voice already installed on your Mac. **She speaks but does not listen** — there
is no speech recognition, no microphone access, and the recording indicator will
never appear because of this app. Synthesis needs no permission; only
recognition does, and there is none here. You can switch the voice off.

## Your licence

Keys are verified offline using a cryptographic signature checked against a
public key inside the app. Entering one makes **no network request**, so we do
not learn that you installed it, when you run it, or how you use it. The trade
is deliberate: a check that phoned home would need a server, a server would need
an account, and the promise above would be gone.

Your key is bound to the email you bought with. That is the only personal
information involved, and it lives in our email, not in the app.

## What we collect when you buy

To sell you a licence we receive **your name and email address**, because you
send them to us in an email, and we keep them to issue your key and to support
you afterwards. That is the only personal data we hold, and for it we are the
data controller.

- **Why:** to perform our contract with you, and to keep tax records.
- **How long:** as long as your licence is valid, plus any period tax law
  requires.
- **Who else sees it:** our email provider. We do not sell it, and we do not
  send marketing unless you ask.
- **Your rights:** access, correction, deletion, portability, objection. Email
  [SUPPORT EMAIL] and we will act within 30 days.

## The website

This page is served by **GitHub Pages, which logs the IP address of every
visitor**. We cannot switch that off and we do not see those logs; GitHub uses
them for security and abuse prevention. [GITHUB PAGES PRIVACY LINK]

[FONT DISCLOSURE — delete this paragraph once fonts are self-hosted: The site
currently loads fonts from Google's servers, which means Google receives your IP
address when the page loads. We are removing this.]

There are no cookies, no analytics, no tracking pixels and no third-party
scripts beyond the above.

## Children

Not directed at children under 16, and we do not knowingly collect their data.

## Changes

If we change what the app does, this page changes in the same release — that is
a rule we now hold ourselves to, having broken it once. The "last updated" date
above tells you when.

## Contact

[TRADER NAME], [TRADER ADDRESS] — [SUPPORT EMAIL]

If you are in the EU or UK and think we have handled your data wrongly, you may
complain to your national data protection authority.
