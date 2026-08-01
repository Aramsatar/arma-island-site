# Before you publish any of these

Six drafts, written against what ARMA Island **actually does** — every factual
claim in them was checked against the source and the signed binary, not
assumed. That is the part templates cannot give you, and it is also why they
need your decisions before they go up.

**I am not a lawyer.** These are careful drafts, not legal advice. The clause
most worth a professional eye is the EU right-of-withdrawal waiver in the refund
policy: get it wrong and you owe refunds for 14 days on every sale regardless of
what the page says.

---

## Fill these in before publishing — the documents will not work without them

| Placeholder | What it needs | Why it is not optional |
|---|---|---|
| `[TRADER NAME]` | Aram Satar, until the OÜ exists | EU law requires a named trader |
| `[TRADER ADDRESS]` | a real geographical address | required; a PO box is not enough |
| `[TRADER PHONE]` | a working number | required alongside email |
| `[SUPPORT EMAIL]` | the address you will actually read | it is the legal contact |
| `[GOVERNING LAW]` | see the note below | decides where a dispute is heard |

**Your site currently identifies no trader at all.** That is the single most
common enforcement trigger for a small seller, and it is a ten-minute fix.

## Two things to fix that are not documents

1. **Google Fonts is loaded from Google's servers**, so every visitor's IP
   address goes to Google before they consent to anything. This is the item that
   has produced actual fines in the EU. Self-host the font files; the fix is
   downloading two files and changing one `<link>`.
2. **GitHub Pages logs visitor IPs** and you cannot switch that off. It belongs
   in the privacy policy, disclosed, rather than contradicted by a claim that you
   collect nothing on the web.

## Decisions only you can make

- **Governing law.** Today you are contracting personally from Iraq. Naming
  Iraqi law will read as unenforceable to an EU consumer and may put buyers off;
  naming a law you have no connection to is not automatically binding either.
  The honest interim: name your own jurisdiction, and state plainly that
  mandatory consumer protections in the buyer's country still apply — which is
  true regardless of what any contract says. Revisit the moment the OÜ exists.
- **Does the site target the EU?** If yes, an Article 27 EU representative is
  required. Today the targeting signals are weak (English only, USD only, no EU
  language, no EUR). Adding EUR pricing or an EU language changes that answer.
- **Cyber insurance** is a purchase, not a document. See `06-`.

## What changes the day the OÜ is formed

The OÜ becomes the contracting party for **new** sales — but it does **not**
automatically take over licences already sold by you personally. Those stay your
obligation unless assigned. Every `[TRADER NAME]` becomes the OÜ, an EU-based
seller gains VAT obligations on EU consumer sales, and the personal-liability
exposure stops accruing. Plan a clean cutover date.

---

*Drafted 2026-08-01 against ARMA Island 1.0.1 (arm64, macOS 14+), commit
`e94228e`. If the app changes, these change with it — that is the whole point.*
