# Terms of Sale and Software Licence — ARMA Island

**Last updated:** [DATE] · **Applies to:** ARMA Island 1.0.1 and later

These terms are between you and **[TRADER NAME]**, [TRADER ADDRESS], contactable
at [SUPPORT EMAIL] and [TRADER PHONE] ("we", "us"). Buying a licence, or using
the trial, means you accept them.

## 1. What you are buying

A perpetual, non-exclusive, non-transferable licence to use ARMA Island on Macs
you own or control, for **US$15, once**. There is no subscription and no renewal.

**Your licence key is tied to the email address you bought with.** It is not
tied to a machine, and we do not count activations — install it on every Mac you
use. Verification happens entirely on your Mac using a cryptographic signature;
it never contacts us, which is why the app works with no internet and why we
cannot see where or whether you installed it.

Do not share your key. It identifies you, and a key posted publicly is one we
may stop honouring in future versions.

## 2. What runs it

- **Apple Silicon Mac** (M1 or later). The app is arm64-only and **will not
  launch on an Intel Mac**, whatever macOS version it runs.
- **macOS 14.0 or later.**
- A notch is *not* required. On a Mac without one, the app draws its own pill in
  the same position.

Check these before buying. They are also the grounds on which we refund without
argument — see the Refund Policy.

## 3. The trial

Fourteen days, the full app, no key and no payment details. When it ends the app
stops working until you enter a key.

We have not tried to make the trial tamper-proof, and you could extend it if you
wanted to. We would rather trust you than treat you as a suspect. Doing so is
still a breach of these terms.

## 4. What the app does on your Mac

ARMA Island is not sandboxed — the sandbox would break its three core features —
so it can do more on your Mac than a Mac App Store app. In plain terms it:

- **reads your clipboard continuously** and keeps a history on your disk
  (on by default; see the Privacy Policy for what it refuses to record, and how
  to turn it off),
- **reads coding-agent session files**, including prompt text and the commands
  those agents ran,
- **modifies `~/.claude/settings.json`** to install its hooks, and writes two
  small executables it uses to receive events,
- **sends Apple Events** to Spotify, Music, Chrome and terminal apps to read what
  is playing and to jump to a session — which, for Chrome, means it can see your
  window and tab titles.

macOS will ask your permission for the Apple Events part the first time. The
rest happens because you installed a non-sandboxed app, which is why we are
telling you here rather than burying it.

## 5. What you may not do

Resell, rent, sublicense or redistribute the app; remove or work around the
licence check; or ship it as part of another product. You may not decompile it
except where that right cannot lawfully be excluded.

## 6. Updates

Updates are included when we publish them, and they arrive by download — there
is no auto-updater, because an auto-updater needs a server and a server would
end the privacy promise in section 4 of the Privacy Policy. We are not obliged
to publish updates, and a future major version may be a separate purchase. If it
is, we will say so before you pay.

## 7. Warranty, and what we do not promise

The app is provided **as is**. We do not warrant it will be uninterrupted,
error-free, or fit for a particular purpose.

Specifically: it relies on macOS behaviour that Apple can change without notice,
including a private now-playing interface. **Apple has been tightening this, and
a macOS update may break the now-playing feature permanently.** We will try to
adapt. We cannot promise to succeed, and that is not grounds for a refund
outside the periods in the Refund Policy.

**None of this removes rights you have by law.** If you are a consumer, your
statutory rights — including that the software be as described and of
satisfactory quality — apply whatever this section says.

## 8. Liability

To the extent the law allows, our total liability for any claim relating to the
app is limited to **what you paid for it**. We are not liable for lost data,
lost profits, or indirect losses.

We do not exclude liability for death or personal injury caused by negligence,
for fraud, or for anything else that cannot lawfully be excluded.

**Back up your work.** The app touches your clipboard and another tool's
configuration file; a bug there could lose you something. Section 8 limits what
we owe you, and a backup is what actually protects you.

## 9. Ending the licence

You may stop using the app at any time. We may end your licence if you breach
these terms materially and do not fix it within 14 days of us telling you. If we
do, you delete the app; nothing else follows.

## 10. Law and disputes

These terms are governed by [GOVERNING LAW]. **If you are a consumer in the EU,
UK, or anywhere with mandatory consumer protections, those protections apply to
you regardless of this clause, and you may bring proceedings in your own
country.** We would rather sort a problem out by email first — [SUPPORT EMAIL].

## 11. Changes

We may change these terms for future purchases. The terms you accepted when you
bought are the ones that govern your licence; we will not change them
retroactively to your disadvantage.
