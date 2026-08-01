# Cyber insurance — a decision, not a document

**Last updated:** [DATE]

The video that prompted these six items listed cyber insurance alongside five
documents. It is not a document. You cannot draft it, and drafting something
that looks like one would be the worst outcome — a page implying cover you do
not have.

So this file is the decision, with the numbers, so you can make it once.

## What it would actually cover

Insurance responds to *your* liability when data you are responsible for is
exposed. The claims are: notifying affected people, forensics, legal defence,
regulatory fines where insurable, and business interruption.

## Your exposure, honestly assessed

Small — smaller than the video's audience, and for a structural reason.

**The app holds nothing of yours to lose.** No server, no database, no account
system. Since 1.0.1 it has no network entitlement at all, so customer clipboard
history, agent sessions and now-playing data never leave the customer's Mac.
A breach of *your* systems cannot expose them, because you never had them.

**What you actually hold** is a list of buyer names and email addresses, in your
Gmail, and the private key that signs licences.

That gives three realistic bad days:

| Scenario | Consequence | Insurance helps? |
|---|---|---|
| Your email is compromised → buyer list leaks | Notification duty; reputational | Yes, modestly |
| **Your Ed25519 private key leaks** | Anyone can mint valid licences; revenue gone | **No — this is a revenue loss, not a liability** |
| A defect in the app damages a customer's data | Claims against you personally | Yes — but so does the liability cap |

The middle row is the one that would actually hurt, and insurance does not touch
it. **Protecting that key is worth more than any policy**: it is not in the repo
today, and it should stay off any machine that browses the web, with an offline
copy somewhere you would still have after a laptop theft.

## The recommendation

**Do not buy cyber insurance yet.** At $15 a sale with no server and no stored
customer content, the premium the video quotes ($200–600/year) is a meaningful
fraction of early revenue against a risk you have largely engineered away.

That advice is honest about its limits: the $200–600 figure and the "personally
liable, not your LLC" framing are **US market assumptions**. You will be an
Estonian OÜ selling from Iraq, where both the premium and the liability picture
differ. Do not port the number.

## What to do instead, in order

1. **Form the OÜ.** Today every obligation in these documents attaches to you
   personally, without limit. A company is cheaper than a policy and does more.
2. **Protect the signing key** — offline backup, not on your daily machine.
3. **Keep the liability cap** in the Terms and the MSA. It is your real
   first line of defence and it costs nothing.
4. **Keep the buyer list small and boring** — name and email only. Never store a
   card number; that is what a merchant of record is for.

## Buy a policy when any of these becomes true

- You run a **server** that holds customer data — a licence server, sync, or
  team features. This is the big one; it converts "we hold nothing" into "we
  hold everything".
- You sign an **MSA with an enterprise customer** who requires it. They often do,
  and then it is a cost of the deal rather than a judgement call.
- Revenue makes the premium a rounding error rather than a decision.
- You take payments directly rather than through a merchant of record.

## If you do buy

Ask for: first-party breach response (forensics, notification), third-party
liability, and **technology errors & omissions** — E&O is the part that responds
when your software damages a customer, which is your likeliest claim. Check the
territorial scope actually covers customers outside your own country; a policy
that only covers domestic claims is no use when your buyers are worldwide.

---

**Decision:** not now. Revisit when a server exists, or at the first enterprise
contract — whichever comes first.
