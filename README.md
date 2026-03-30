<div align="center">

<br/>

```
 ███████╗ █████╗ ███╗   ██╗██╗████████╗██╗███████╗███████╗ ██████╗ ███████╗
 ██╔════╝██╔══██╗████╗  ██║██║╚══██╔══╝██║╚════██║██╔════╝██╔═══██╗██╔════╝
 ███████╗███████║██╔██╗ ██║██║   ██║   ██║    ██╔╝█████╗  ██║   ██║███████╗
 ╚════██║██╔══██║██║╚██╗██║██║   ██║   ██║   ██╔╝ ██╔══╝  ██║   ██║╚════██║
 ███████║██║  ██║██║ ╚████║██║   ██║   ██║   ██║  ███████╗╚██████╔╝███████║
 ╚══════╝╚═╝  ╚═╝╚═╝  ╚═══╝╚═╝   ╚═╝   ╚═╝   ╚═╝  ╚══════╝ ╚═════╝ ╚══════╝
```

### **The Offline Data Redactor**
#### *Zero Cloud · Zero Risk · Zero Leaks*

<br/>

[![Offline](https://img.shields.io/badge/Works-100%25%20Offline-00e5c3?style=for-the-badge)](https://github.com/avinashwalton/sanitizeos)
[![No Cloud](https://img.shields.io/badge/Cloud%20Uploads-ZERO-ff4d6d?style=for-the-badge)](https://github.com/avinashwalton/sanitizeos)
[![Price](https://img.shields.io/badge/Lifetime%20License-$25%20Once-fbbf24?style=for-the-badge)](https://avinashwalton.gumroad.com/l/SanitizeOS)
[![No Dependencies](https://img.shields.io/badge/Dependencies-ZERO-a78bfa?style=for-the-badge)](https://github.com/avinashwalton/sanitizeos)
[![Single File](https://img.shields.io/badge/Single-HTML%20File-60a5fa?style=for-the-badge)](https://github.com/avinashwalton/sanitizeos)

<br/>

> **"I deal with SSNs and tax records every day. The fact that nothing gets uploaded anywhere is a game-changer. My compliance officer loves it."**
> — *Sarah R., HR Director, Fortune 500*

<br/>

**[⚡ Try Free Demo](https://avinashwalton.github.io/SanitizeOS)** &nbsp;&nbsp;·&nbsp;&nbsp; **[🔓 Get Lifetime Access — $25](https://avinashwalton.gumroad.com/l/SanitizeOS)** &nbsp;&nbsp;·&nbsp;&nbsp; **[📖 How It Works](#how-it-works)**

<br/>

</div>

---

<br/>

## 🚨 The Problem Nobody Talks About

Every time you paste a client document into a cloud-based redaction tool, **you are doing this:**

```
Your Client's SSN  ──────►  Your Browser
                                  │
                                  ▼
                         HTTP POST /api/redact
                                  │
                                  ▼
                      ┌───────────────────────┐
                      │   Third-Party Server  │  ← Who owns this?
                      │   (You don't know     │  ← What do they log?
                      │    what happens here) │  ← Who has access?
                      └───────────────────────┘
                                  │
                                  ▼
                      Your client's data sits in
                      someone else's database.
                      Even "temporarily."
```

Cloud redaction tools upload your clients' most sensitive information — Social Security Numbers, credit card numbers, legal case details, medical records — to servers **you have zero control over.**

That's not a workflow. That's a liability.

<br/>

---

<br/>

## ✅ How SanitizeOS Works Instead

```
Your Client's SSN  ──────►  Your Browser
                                  │
                          JavaScript Engine
                          (Regex runs locally)
                                  │
                                  ▼
                      ┌───────────────────────┐
                      │     YOUR MACHINE      │  ← You own this
                      │   (Nothing leaves)    │  ← Zero network calls
                      │                       │  ← Fully auditable
                      └───────────────────────┘
                                  │
                                  ▼
                         Clean Redacted File
                         Downloaded to YOUR disk.

                    Network Requests Made: ZERO.
```

**Open DevTools → Network tab → Paste any text → Watch: nothing fires.**

That's the architecture. Not a marketing claim — verifiable in 10 seconds.

<br/>

---

<br/>

## 🎯 Who Is This For?

<table>
<tr>
<td width="33%" valign="top">

### ⚖️ Legal Professionals
Attorneys, paralegals, and law clerks who need to share sanitized case documents — but cannot risk transmitting client SSNs, financial data, or case details to external servers.

**Use case:** Redact client intake forms before forwarding to co-counsel or court filing vendors.

</td>
<td width="33%" valign="top">

### 👔 HR Professionals
HR managers and payroll teams who regularly handle employee records, offer letters, and onboarding documents containing sensitive PII that must be masked before sharing with vendors.

**Use case:** Sanitize payroll exports before sending to third-party benefits platforms.

</td>
<td width="33%" valign="top">

### 🧾 Accountants & CPAs
Public accountants and tax professionals who process client financial data and need a clean, auditable way to remove PII from spreadsheets before sharing with colleagues or clients.

**Use case:** Strip SSNs and card numbers from CSV exports before analyst review.

</td>
</tr>
</table>

<br/>

---

<br/>

## ⚔️ SanitizeOS vs. Cloud Redaction Tools

> *Why pay a subscription to hand your clients' data to strangers?*

| | 🛡️ SanitizeOS | ☁️ Cloud Tools |
|---|:---:|:---:|
| Data stays on your device | ✅ Always | ❌ Never |
| Works without internet | ✅ Yes | ❌ No |
| No account or signup required | ✅ Yes | ❌ No |
| Zero server-side data processing | ✅ Guaranteed | ❌ Core business model |
| Auditable — read the source code | ✅ Open | ❌ Black box |
| Air-gap compatible | ✅ Yes | ❌ No |
| GDPR-safe data pipeline | ✅ By design | ⚠️ Depends on their ToS |
| HIPAA-safe data pipeline | ✅ By design | ⚠️ Requires BAA agreement |
| Works during internet outages | ✅ Always | ❌ Never |
| No subscription fee | ✅ $25 once | ❌ $X/month forever |
| No renewal risk | ✅ Own it forever | ❌ Service can shut down |
| No data breach risk from vendor | ✅ Zero | ❌ Real and ongoing |

<br/>

---

<br/>

## 🔍 What Gets Detected & Redacted

SanitizeOS uses battle-tested regular expressions to detect 6 types of Personally Identifiable Information (PII):

```
INPUT                              OUTPUT
─────────────────────────────────────────────────────────────
john.doe@acmecorp.com         →    [REDACTED-EMAIL]
(212) 555-0147                →    [REDACTED-PHONE]
+1-917-867-5309               →    [REDACTED-PHONE]
572-88-3419                   →    [REDACTED-SSN]
4111 1111 1111 1111           →    [REDACTED-CARD]
5500-0000-0000-0004           →    [REDACTED-CARD]
3714 496353 98431             →    [REDACTED-CARD]
192.168.0.45                  →    [REDACTED-IP]
03/14/1985                    →    [REDACTED-DATE]
YOUR CUSTOM KEYWORD           →    [REDACTED]  ← Premium
─────────────────────────────────────────────────────────────
```

**Supported formats:**
- 📧 **Emails** — all standard RFC 5322 formats
- 📞 **Phone Numbers** — US & UK, with/without country code, all separators
- 🪪 **US SSNs** — `XXX-XX-XXXX`, `XXX XX XXXX`, unformatted
- 💳 **Credit Cards** — Visa, Mastercard, Amex, Discover, spaced or unspaced
- 🌐 **IP Addresses** — IPv4 (all ranges)
- 📅 **Dates** — MM/DD/YYYY, MM-DD-YYYY formats

<br/>

---

<br/>

## 📦 What's Included

<table>
<tr>
<td width="50%" valign="top">

### 🆓 Free Demo (`index.html`)
*Available on GitHub — no payment required*

- ✅ Live text redaction (real-time)
- ✅ All 6 PII types detected
- ✅ Copy output to clipboard
- ✅ Detection count stats per type
- ✅ Sample text to test instantly
- ❌ File upload
- ❌ Download output
- ❌ Bulk CSV processing
- ❌ Custom keyword rules

</td>
<td width="50%" valign="top">

### 🔓 Full Tool (`tool.html`) — $25 Lifetime
*Delivered via Gumroad after purchase*

- ✅ Everything in free, plus:
- ✅ **Drag & drop file uploads** (.txt, .csv)
- ✅ **Multiple files at once** — batch processing
- ✅ **Download redacted files** (auto-named)
- ✅ **Custom Rules tab** — add your own keywords/regex
- ✅ **IP Address & Date detection** (6 total types)
- ✅ **Session history** — log of all redactions
- ✅ **Toggle each rule on/off** independently
- ✅ **Air-gap ready** — no internet ever needed
- ✅ Future updates included

</td>
</tr>
</table>

<br/>

---

<br/>

## 🚀 How It Works

**Free demo — zero setup:**

```bash
# Clone and open. That's literally it.
git clone https://github.com/avinashwalton/SanitizeOS.git
open index.html
```

No `npm install`. No build step. No Node. No Python. No Docker.
Just double-click `index.html` and it works.

**Paid tool — same simplicity:**
1. Purchase on [Gumroad](https://avinashwalton.gumroad.com/l/SanitizeOS)
2. Download `tool.html` from your Gumroad receipt
3. Double-click it. Done.

**For air-gapped environments:**
```
1. Download tool.html on any internet-connected machine
2. Copy to USB drive
3. Transfer to air-gapped machine
4. Open in any browser
5. Works perfectly with zero internet
```

<br/>

---

<br/>

## 🏗️ Technical Architecture

```
tool.html (Single File)
│
├── HTML5 Structure
│   └── 4 tabs: Text · File · Rules · History
│
├── CSS3 Styling
│   ├── Dark mode glassmorphism UI
│   ├── CSS custom properties (variables)
│   ├── Responsive — mobile + desktop
│   └── Zero external CSS dependencies
│
├── Vanilla JavaScript Engine
│   ├── RegEx pattern matching (6 PII types)
│   ├── FileReader API (local file processing)
│   ├── Blob + URL.createObjectURL (downloads)
│   ├── Custom rules engine (user-defined)
│   └── Session history (in-memory only)
│
└── External Resources
    └── Google Fonts (display only, optional)

Network Requests to Process Your Data: ZERO
Third-Party SDKs with Data Access:     ZERO
Cookies Set:                           ZERO
localStorage Written:                  ZERO
```

**Tech stack:** Pure HTML · CSS · Vanilla JS · Single file · Zero dependencies

<br/>

---

<br/>

## 💰 Pricing

<div align="center">

| Plan | Price | File Processing | Custom Rules | Downloads |
|------|-------|:-:|:-:|:-:|
| **Free Demo** | $0 | ❌ | ❌ | ❌ |
| **Lifetime License** | **$25 once** | ✅ | ✅ | ✅ |

<br/>

### **[🔓 Get Lifetime Access on Gumroad — $25](https://avinashwalton.gumroad.com/l/SanitizeOS)**

*Pay once. Own it forever. No subscription. No renewal. No gotchas.*
*30-day no-questions-asked refund guarantee.*

</div>

<br/>

---

<br/>

## 💬 What Users Say

> *"Our firm handles client SSNs and financial records. I needed a tool I could run on an air-gapped machine. SanitizeOS is exactly that — and the price is a no-brainer."*
> — **Michael K., Tax Attorney**

> *"Redacted 3,000 rows of client data from a CSV in seconds. Worth every penny for the peace of mind alone."*
> — **Priya T., CPA, Public Accounting**

> *"I checked the network tab. Zero requests. That's when I knew this was different from every other tool I'd tried."*
> — **David L., IT Compliance Manager**

<br/>

---

<br/>

## ❓ Frequently Asked Questions

<details>
<summary><strong>Does my data really never leave my device?</strong></summary>
<br/>
Yes. SanitizeOS uses the browser's built-in JavaScript engine to run regex patterns on your text locally. There is no backend server, no API endpoint, no fetch() call, and no WebSocket. You can verify this yourself in 10 seconds: open DevTools → Network tab → paste sensitive text → watch nothing fire.
<br/><br/>
</details>

<details>
<summary><strong>Can I use the paid tool.html on a machine with no internet?</strong></summary>
<br/>
Yes, that's a core design goal. After downloading tool.html once, copy it to any machine — including air-gapped workstations. It requires no internet connection to process files or redact text. Even the fonts gracefully fall back to system fonts if unavailable offline.
<br/><br/>
</details>

<details>
<summary><strong>What's the difference between the free demo and the paid tool?</strong></summary>
<br/>
The free demo (index.html) lets you paste text and see it redacted live — great for quick one-off sanitization. The paid tool (tool.html) adds file upload (.txt and .csv), bulk processing, downloadable output, a custom rules engine for your own keywords/patterns, per-rule toggles, and session history.
<br/><br/>
</details>

<details>
<summary><strong>How do I receive the paid tool after purchase?</strong></summary>
<br/>
Gumroad delivers it automatically. After payment, you'll receive an email with a download link for tool.html. No account needed, no app to install — just the single HTML file.
<br/><br/>
</details>

<details>
<summary><strong>Is this GDPR / HIPAA compliant?</strong></summary>
<br/>
Since your data never leaves your device, SanitizeOS eliminates the cloud upload risk that most GDPR and HIPAA guidance focuses on. For GDPR, processing data locally means no third-party data processor is involved. For HIPAA, there's no covered entity or business associate receiving PHI. That said, compliance is holistic — always consult your compliance officer for your specific workflow.
<br/><br/>
</details>

<details>
<summary><strong>Can I inspect the source code before buying?</strong></summary>
<br/>
The free demo (index.html) is fully open source right here on GitHub. The paid tool uses the same architecture — just more of it. You can verify the security model of the free version, and the paid version follows identical principles.
<br/><br/>
</details>

<details>
<summary><strong>What if the regex misses something or has false positives?</strong></summary>
<br/>
The patterns are tuned for the most common US/UK formats. For edge cases, the paid version includes a Custom Rules tab where you can add your own patterns. You're always in control — you can toggle any rule on or off independently.
<br/><br/>
</details>

<br/>

---

<br/>

## 🗺️ Roadmap

- [x] Live text redaction (6 PII types)
- [x] File upload and download (.txt, .csv)
- [x] Custom keyword / regex rules
- [x] Session history
- [x] Per-rule toggles
- [ ] PDF text extraction + redaction
- [ ] Redaction audit log export
- [ ] Multi-file batch zip download
- [ ] Named entity detection (basic NLP)
- [ ] Windows `.exe` wrapper (Electron)

> All future updates are included with the $25 lifetime license.

<br/>

---

<br/>

## 📜 License

This repository contains the **free demo version** (`index.html`) for evaluation purposes.

The full licensed tool (`tool.html`) is a **commercial product** available at:
👉 **[https://avinashwalton.gumroad.com/l/SanitizeOS](https://avinashwalton.gumroad.com/l/SanitizeOS)**

The free demo may be used and shared freely. The paid tool is licensed for individual use by the purchaser on their own devices.

<br/>

---

<br/>

<div align="center">

**Built for professionals who take client confidentiality seriously.**

If you've read this far, you already know the answer.

<br/>

### **[🔓 Get Lifetime Access — $25](https://avinashwalton.gumroad.com/l/SanitizeOS)**

*One file. One payment. Zero risk.*

<br/>

---

Made with ❤️ in India by **[Avinash Walton](https://github.com/avinashwalton)**

*If SanitizeOS saved you from a compliance headache, consider leaving a ⭐ on GitHub.*

</div>
