https://medo.dev/projects/app-bsdkf2x9s0sh/preview

# ⬡ AutoPenAI

> **AI-Powered Autonomous Penetration Testing Dashboard**  
> Built at **Milan AI Week Hackathon 2026**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-medo.dev-00ff88?style=for-the-badge&logo=vercel&logoColor=black)](https://medo.dev/projects/app-bsdkf2x9s0sh/preview)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)]()

---

## 🔗 Live Preview

**[→ Open AutoPenAI](https://medo.dev/projects/app-bsdkf2x9s0sh/preview)**

---

## 📖 What is AutoPenAI?

AutoPenAI is a fully autonomous penetration testing dashboard powered by Claude AI. It simulates a complete red-team engagement — from reconnaissance to final report — entirely in the browser, with a human-in-the-loop approval gate before any exploitation is attempted.

No backend. No manual commands. Just enter a target, give consent, and the AI does the rest.

> ⚠️ **Authorized use only.** AutoPenAI is built for ethical, consent-first security testing. Never use it against targets you do not own or have explicit permission to test.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🎯 **Reconnaissance** | AI simulates host discovery, port scanning, service fingerprinting |
| 🔍 **Vulnerability Assessment** | Claude identifies real CVEs with CVSS scores for discovered services |
| 💥 **Exploit Research** | AI maps exploitable vectors and success probabilities |
| 🔐 **Approval Gate** | Full stop at Phase 5 — human must approve before exploitation |
| 📊 **Live Activity Log** | Real-time streaming log of every AI action |
| 📈 **Phase Tracker** | Visual 7-phase progress tracker in the sidebar |
| 🤖 **Exploit Simulation** | Claude simulates attack chains with consent, captures findings |
| 📝 **Streamed Report** | AI writes a full markdown pentest report word by word |
| ⬇️ **Download Report** | Export the complete `.md` report to your machine |

---

## 🧠 How It Works

AutoPenAI runs a 7-phase autonomous penetration testing pipeline, each phase powered by real Claude API calls:

```
Phase 1 → Reconnaissance          Discover hosts, ports, services
Phase 2 → Scanning & Enumeration  Deep service fingerprinting, banner grabs
Phase 3 → Vulnerability Assessment CVE lookup, CVSS scoring via AI
Phase 4 → Exploit Research         Match exploits to vulnerabilities
Phase 5 → Exploitation (Gated)    ⚠ HUMAN APPROVAL REQUIRED
Phase 6 → Post-Exploitation        Lateral movement, privilege paths
Phase 7 → Report Generation        Full AI-authored pentest report
```

---

## 🖥️ Dashboard UI

The dashboard includes:

- **Left sidebar** — Target configuration form, consent checkbox, phase tracker
- **Main panel** — Live activity log, vulnerability findings table (CVE ID / Severity / CVSS / Description), exploit simulation results, streamed final report
- **Approval Gate** — A hard stop with Approve / Decline buttons before any exploit runs
- **Download button** — Saves the full report as a `.md` file

---

## 🚀 Getting Started

### Run Locally

```bash
# Clone the repo
git clone https://github.com/your-username/autopenai.git
cd autopenai

# Install dependencies
npm install

# Start the dev server
npm run dev
```

### Requirements

- Node.js 18+
- A modern browser
- Claude API access (via Anthropic) — the app calls `api.anthropic.com` directly

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React (JSX) |
| AI Engine | Claude Sonnet (`claude-sonnet-4-20250514`) |
| Styling | Inline CSS + Google Fonts (Orbitron, Share Tech Mono, Rajdhani) |
| API | Anthropic `/v1/messages` with streaming |
| Deployment | [Medo.dev](https://medo.dev) |

---

## ⚙️ Configuration

The app uses the Anthropic API directly from the browser. To use it in your own environment:

1. Set up your Anthropic API key in your deployment environment
2. The app targets `claude-sonnet-4-20250514` — update the model string in `AutoPenAI.jsx` if needed
3. Adjust the default port list and scan parameters in the component state

---

## 🔒 Ethics & Safety

AutoPenAI is built with a **consent-first architecture**:

- The scan will not launch without the operator checking the authorization consent box
- Exploitation is gated behind a mandatory human approval step
- All activity is logged with timestamps
- Scope is configured before any phase begins

This tool is intended for:
- ✅ CTF (Capture the Flag) challenges
- ✅ Your own lab environments
- ✅ Systems you have written permission to test
- ❌ Never for unauthorized targets

---

## 🏆 Hackathon

Built in 24 hours at **Milan AI Week Hackathon 2026**.

---

## 📄 License

MIT — free to use, modify, and distribute with attribution.

---

<p align="center">
  Made with ⬡ AutoPenAI &nbsp;·&nbsp;
</p>
