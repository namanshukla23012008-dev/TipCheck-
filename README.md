# 🛡 TipCheck+ : Read the tip. Not the hype.

> An open-source, explainable financial-message literacy tool. Paste a forwarded investment tip and see **which words are red flags and why**. English + हिन्दी. No server, no sign-up, no data leaves your browser.

**🔗 Live demo:** `<add your GitHub Pages URL>`  **🎥 Demo video / slides:** `<add link>`

## 1. The problem
Millions of first-time investors receive "guaranteed return" tips on WhatsApp and Telegram. Most people are not careless; they have nobody to ask in the 60 seconds before they pay. Tools that only say "scam / not scam" teach nothing and are often wrong. TipCheck+ **explains** instead of judging.

## 2. Features
- **Red-flag meter (0-100)** with the exact **quotes** that triggered each flag and a plain-language reason (guaranteed returns, pressure, secrecy, "money multiplies" claims, pay-to-join, OTP/link requests, unverified registration claims).
- **Hindi / English** interface and Hindi/Hinglish patterns (e.g. "kal double hoga", "kisi ko mat batana").
- **Verify independently** checklist with SEBI reference link.
- **Warn your family:** a calm, forwardable message (copy, WhatsApp share, read-aloud).
- **"Already paid?"** panel: call cybercrime helpline **1930** and report at cybercrime.gov.in.
- **60-second literacy coach** quiz: spot hype vs information.
- **Private by design:** runs 100% in your browser; nothing is uploaded or stored.
- **Honest:** the score is a heuristic, not scam probability. "Promotion" does not mean fraud; "no flags" does not mean safe. Education only, not investment advice.

## 3. How it works (transparent, no black box)
All logic lives in one readable `index.html`: a list of weighted rules (`R`) with bilingual explanations, a "money multiplier" detector (amount in vs promised amount out), and a scoring function. Anyone can read, audit and improve it.

## 4. Setup guide (run locally)
No installation needed.
```bash
git clone https://github.com/<your-username>/tipcheck-plus.git
cd tipcheck-plus
open index.html        # Mac   (Windows: double-click index.html)
```
Optional local server: `python3 -m http.server 8000` then open http://localhost:8000

## 5. Deploy (free, GitHub Pages)
Repo **Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)` → Save.** Your site goes live at `https://<your-username>.github.io/tipcheck-plus/`.

## 6. Why open innovation matters
Scam-literacy tools are usually closed products you must trust blindly. Open source lets **anyone audit the rules, add new scam patterns, and translate to their language**, so every contribution protects another community. TipCheck+ contributes: (1) an open, explainable rule set for Indian financial-scam patterns, (2) Hindi/Hinglish patterns and examples, (3) a one-file template other regions can fork by swapping SEBI for their own regulator.

## 7. Community
See [CONTRIBUTING.md](CONTRIBUTING.md). Good first issues: new rules, new languages, quiz questions. PRs and issues welcome.

## 8. Roadmap
More Indian languages · screenshot reading · optional open-weight model (e.g. Gemma) for deeper, context-aware explanations · community-maintained pattern library · browser extension.

## Disclaimer
Educational only. Not investment or legal advice. Scores are heuristic. Do not paste personal details.

**License:** Apache-2.0 (see [LICENSE](LICENSE)).
