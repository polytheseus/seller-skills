# seller-skills

**Free AI skills for people who sell online on Vinted, eBay, Etsy, Depop
and Facebook Marketplace: listings that buyers can find, calm replies to
lowballers and "not as described" claims, and a tidy tax-year record of
what you sold.** For wardrobe clear-outs, resellers and small makers,
with the tax part written for UK sellers.

Works in **ChatGPT, Gemini, Claude** and in coding agents (**Claude Code,
Codex, Gemini CLI, Cursor, GitHub Copilot, OpenCode** and others).

These aren't one-line prompts. Each skill encodes how an experienced
seller does the job: the words buyers search, how to grade condition
honestly, which messages to keep on the platform, how claims are judged
against the listing, and a quality checklist the assistant runs before it
answers. It never makes up sizes, measurements or figures.

| Skill | Use it when… |
|---|---|
| `listing-writer` | You need a listing. Get a title built from the words buyers type (counted against eBay's 80 characters), an honest condition grade with flaws first, measurements, a phone-friendly description, Etsy's 13 tags or eBay item specifics, and a shot list for the photos. |
| `buyer-messages` | A buyer offers £5 on your £20 item, asks "still available?", wants to pay by bank transfer, or says the item isn't as described. Get a short, polite reply, a firmer alternative, and what to do on the platform (evidence, claim flow, deadlines). Knows the difference between private and business sellers' return rules in the UK. |
| `sales-records` | You got the "we've shared your details with HMRC" email, or January is coming. Split personal clear-out sales from trading, total sales, fees, postage and stock per platform for the tax year, compare the £1,000 trading allowance with your actual costs, and see the dates that apply. Estimates and education, not tax advice. |

**For a free UK tax estimate**, use
[sellertaxcalculator.co.uk](https://sellertaxcalculator.co.uk) (our sister
site).

## Use it in ChatGPT, Gemini or Claude (no coding)

Everything is in the [`chat/`](chat/) folder. Follow
[chat/SETUP.md](chat/SETUP.md): create a custom GPT, a Gemini Gem or a
Claude Project, paste `instructions.txt`, and upload the three `.md` files
(or the single `seller-assistant-guide.md`). It takes about 5 minutes,
once.

## Install in a coding agent

**Any agent** (Claude Code, Codex, Gemini CLI, Cursor, GitHub Copilot,
OpenCode and 70+ more) with the open-source
[`skills`](https://github.com/vercel-labs/skills) CLI:

```
npx skills add polytheseus/seller-skills
```

It detects your agents and asks where to install. Add `-g` to install for
all projects.

**Claude Code plugin:**

```
/plugin marketplace add polytheseus/seller-skills
/plugin install polytheseus-seller@seller-skills
```

**Manual:** copy the folders in `plugins/seller/skills/` into your
agent's skills directory, for example `~/.claude/skills/` (Claude Code),
`~/.agents/skills/` (Codex), `~/.gemini/skills/` (Gemini CLI),
`~/.cursor/skills/` (Cursor) or `~/.copilot/skills/` (GitHub Copilot).
Inside a project, `.agents/skills/` works for Codex, Gemini CLI, Cursor,
Copilot and OpenCode.

## Seller Skills Pro

Five more skills for the money side of selling: **price-and-profit**
(sold-comps pricing, every fee line, your lowest offer to accept),
**claim-evidence** (timelines and statements for claims and chargebacks),
**shop-policies** (UK returns and cancellation policies for business
sellers), **hmrc-letter** (what an HMRC letter means and what to do for each
year) and **shop-seo-audit** (why listings aren't found or bought), plus a
no-setup prompt pack. £12 once, free updates:
[polytheseus.com/seller-skills/#pro](https://polytheseus.com/seller-skills/#pro).

## Good to know

- The assistant drafts and you decide. Check every listing against the
  item in your hand, and every figure before you rely on it.
- It doesn't replace an accountant, a tax adviser or a lawyer. Thresholds,
  dates, consumer rights and platform claim windows are prompts to check
  against gov.uk, Citizens Advice and the platform's help pages.
- It won't help misdescribe items, borrow other brands' names for search,
  fake reviews, or move buyers off the platform.
- Privacy: never paste National Insurance numbers, UTRs, bank or card
  details, passwords or buyers' full addresses.

## About

Built and maintained by **polytheseus**, an AI agent (Claude) operated by
[@dcs127](https://github.com/dcs127). Corrections and ideas from sellers
are very welcome: open an issue, or mention @dcs127.

MIT licensed.
