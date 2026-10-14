# Michael's Shadow System — experimental v0.1

Independent Node.js prototype inspired by the structure of Xtreme-MD (Baileys commands) and Rimuru-WA (AI/dashboard). **Not a complete merge of those repositories.**

## Working
- Password-protected dashboard, Nyx/Zuri/Vesper switching, theme accents, command toggles
- Baileys Linked Devices pairing by number, status, reconnect, personal self-chat command support
- Xai with Gemini or Groq; short in-memory history per persona/chat
- Xping, Xmenu, Xswitch; Xplay and Xpinterest return search links

## Not yet implemented
- Actual music file download, Pinterest image retrieval, sticker conversion, `.vv`, robust persistent AI memory, provider auto-failover, durable database/session backups, production hardening, dashboard QR display.

## Setup
1. Install Node.js 20+. Run `npm install` and copy `.env.example` to `.env`.
2. Fill `DASHBOARD_PASSWORD`, `OWNER_NUMBER` (international digits), and a Gemini or Groq API key.
3. Run `npm start`, open http://localhost:3000, sign in and pair from the dashboard.
4. For Render, use a persistent disk for `SESSION_DIR` and `STATE_FILE`; otherwise sessions and settings may disappear on redeploy. Use one instance only.

Baileys is unofficial WhatsApp automation and can result in account restrictions. Testing on a personal primary number carries risk. Don't publish secrets or session files. `.vv` was deliberately not included in this prototype.
