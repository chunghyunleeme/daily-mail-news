# daily mail news

> Your inbox, turned into daily news at 8 AM.

**daily mail news** is a personal email intelligence service that summarizes  
**your own inbox** from the previous day and delivers it every morning at **8 AM (local time)**.

It helps you start the day by reading your email like news —  
only the important signals, without inbox noise.

---

## ✨ What It Does

- Collects emails from your inbox (starting with Gmail)
- Classifies emails by importance
  - **KEEP**: needs your attention
  - **SUMMARY**: informational
  - **DROP**: low-signal noise
- Archives non-essential emails automatically
- Generates a single daily summary
- Delivers the summary **every morning at 8 AM (your local time)**

This is not real-time notifications.  
This is a **daily briefing**.

---

## ⏰ Daily Delivery Policy

- **Scope**: Emails received **yesterday (00:00–23:59)**
- **Delivery Time**: **08:00 AM**, based on the user’s local timezone
- **Frequency**: Once per day

The goal is simple:
> Know what matters *before* your workday starts.

---

## 📬 Summary Email Example


📬 Yesterday’s Mail News

🔴 Needs Attention

Product Sync meeting tomorrow at 10:30 (Zoom)

Finance team: budget confirmation requested

🟡 For Reference

GitHub: 3 PRs merged

Stripe: daily payment report (no issues)

⚪ Auto-Archived

Promotions: 14 emails

yaml
Copy code


If you read this, you already know enough.

---

## 🧠 Design Principles

- **Inbox ≠ Task Manager**
- **No real-time alerts**
- **One calm briefing per day**
- **Minimal data retention**
- **Explainable automation**
  - You can always see *why* an email was classified or archived

---

## 📮 Supported Mail Providers

Initial support:
- **Gmail** (including Google Workspace)

Planned expansions:
- Outlook / Microsoft 365
- Naver Mail
- IMAP-based enterprise email

Mail providers are abstracted to allow seamless future expansion.

---

## 🔔 Notification Targets

- Email (default)

Planned:
- Slack DM
- Push notifications
- Other messaging channels

Mail providers and delivery channels are designed to be independent.

---

## 🛠 Technology Stack

- **Backend**: NestJS
- **ORM**: MikroORM
- **AI / NLP**: LangChain-based LLM pipelines
- **Architecture**: Provider / Adapter-based modular design

> This repository focuses on service architecture and product behavior.  
> Implementation details are intentionally modular and replaceable.

---

## 🔐 Trust & Privacy

- Email content is **not stored permanently**
- Only minimum metadata is persisted
- Emails are processed and discarded after summarization
- Automation can be disabled at any time
- Classification decisions are logged and explainable

This service works for you — not on your data.

---

## 🚧 Project Status

- 🚀 Early development
- 🧪 Initial focus: Gmail + daily summary
- 🧩 Provider and channel expansion planned

---

## 📄 Documentation

- `PRD.md` — Product requirements and scope
- `docs/architecture.md` — High-level system design
- `docs/data-policy.md` — Data handling and privacy
- `docs/classification-v1.md` — Email classification rules

---

## 📌 Disclaimer

daily mail news summarizes **your personal inbox**.  
It is **not affiliated with any news organization**.

---

## 📝 License

MIT
