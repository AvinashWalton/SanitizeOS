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
#### *Zero Cloud · Zero Risk · Zero Leaks · Legal-Grade PII Masking*

<br/>

[![Offline](https://img.shields.io/badge/Works-100%25%20Offline-00e5c3?style=for-the-badge)](https://github.com/avinashwalton/sanitizeos)
[![No Cloud](https://img.shields.io/badge/Cloud%20Uploads-ZERO-ff4d6d?style=for-the-badge)](https://github.com/avinashwalton/sanitizeos)
[![Price](https://img.shields.io/badge/Lifetime%20License-$25%20Once-fbbf24?style=for-the-badge)](https://avinashwalton.gumroad.com/l/SanitizeOS)
[![PII Types](https://img.shields.io/badge/PII%20Types-6%20Detected-a78bfa?style=for-the-badge)](https://github.com/avinashwalton/sanitizeos)
[![Single File](https://img.shields.io/badge/Single-HTML%20File-60a5fa?style=for-the-badge)](https://github.com/avinashwalton/sanitizeos)

<br/>

> **"I checked the network tab. Zero requests. That's when I knew this was different from every other tool I'd tried."**
> — *David L., IT Compliance Manager*

<br/>

**[⚡ Try Free Demo](https://avinashwalton.github.io/sanitizeos)** &nbsp;&nbsp;·&nbsp;&nbsp; **[🔓 Get Lifetime Access — $25](https://avinashwalton.gumroad.com/l/SanitizeOS)** &nbsp;&nbsp;·&nbsp;&nbsp; **[📖 How It Works](#how-it-works)**

<br/>

</div>

---

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

Cloud redaction tools upload your clients' most sensitive information — SSNs, credit cards, legal case details, medical records — to servers **you have zero control over.** That's not a workflow. That's a liability.

---

## ✅ How SanitizeOS Works Instead

```
Your Client's SSN  ──────►  Your Browser
                                  │
                          JavaScript Engine
                          (All regex runs locally)
                                  │
                                  ▼
                      ┌───────────────────────┐
                      │     YOUR MACHINE      │  ← You own this
                      │   (Nothing leaves)    │  ← Zero network calls
                      │                       │  ← Fully auditable
                      └───────────────────────┘
                                  │
                                  ▼
                    Clean Redacted Output + Audit Log
                    Downloaded to YOUR disk.

               Network Requests Made: ZERO. Always.
```

**Open DevTools → Network tab → Paste any text → Watch: nothing fires.**

---

## 🎯 Who Is This For?

<table>
<tr>
<td width="33%" valign="top">

### ⚖️ Legal Professionals
Attorneys, paralegals, and law clerks who share sanitized documents but cannot risk transmitting client SSNs or financial data to external servers.

**Use case:** Redact client intake forms before forwarding to co-counsel or court vendors.

</td>
<td width="33%" valign="top">

### 👔 HR Professionals
HR managers and payroll teams handling employee records, offer letters, and onboarding documents that must be masked before sharing with third parties.

**Use case:** Sanitize payroll exports before sending to benefits platforms.

</td>
<td width="33%" valign="top">

### 🧾 Accountants & CPAs
Tax professionals who process client financial data and need a clean, auditable way to remove PII from spreadsheets before sharing.

**Use case:** Strip SSNs and card numbers from CSV exports before analyst review.

</td>
</tr>
</table>

---

## ✨ Full Feature Set (Paid — `tool.html`)

### 🔍 Core Redaction Engine
The regex engine detects **6 types of PII** and processes them in the correct order to avoid false positives:

```
INPUT                              OUTPUT
─────────────────────────────────────────────────────────────
john.doe@acmecorp.com         →    [REDACTED - EMAIL]
(212) 555-0147                →    [REDACTED - PHONE]
+44 7911 123456               →    [REDACTED - PHONE]
572-88-3419                   →    [REDACTED - SSN]
4111 1111 1111 1111           →    [REDACTED - CARD]
192.168.0.45                  →    [REDACTED - IP]
03/14/1985                    →    [REDACTED - DATE]
YOUR CUSTOM KEYWORD           →    [REDACTED]
─────────────────────────────────────────────────────────────
```

Each PII type can be toggled on/off independently. The detection engine processes matches in a non-overlapping, priority-ordered pass to prevent conflicts between patterns.

---

### 🎨 3 Masking Styles (Legal Standard)

Choose how redacted content is displayed before you run the tool:

| Style | Example Output | Best For |
|-------|---------------|----------|
| **Solid Black Blocks** | `█████████` | Classic legal redaction look |
| **[REDACTED - PII]** | `[REDACTED - EMAIL]` | Labelled, type-specific masking |
| **[CONFIDENTIAL]** | `[CONFIDENTIAL]` | Formal document workflows |

You can switch styles at any time and re-run the redaction instantly.

---

### 👆 Click-to-Reveal (False Positive Fix)

In the output pane, every redacted block renders as a **clickable styled element** — like a black highlighter in a legal document. If the regex accidentally masks something that isn't actually PII:

1. Click the redacted block
2. Original text is revealed (highlighted in green)
3. Click again to re-mask it

No need to re-process the entire document. Works independently on each redacted segment.

---

### 📋 Compliance Audit Log

The Audit Report tab generates a downloadable `.txt` file containing:

```
═══════════════════════════════════════════════
          SANITIZEOS — AUDIT LOG
═══════════════════════════════════════════════

Tool Version  : SanitizeOS Lifetime License
Processing    : 100% Local / Offline
Generated At  : 6/15/2025, 2:34:17 PM
Session ID    : A3B9F2K1

───────────────────────────────────────────────
              REDACTION SUMMARY
───────────────────────────────────────────────

  Email Addresses    : 3
  Phone Numbers      : 2
  US SSNs            : 1
  Credit Card Nos.   : 1
  IP Addresses       : 2
  Dates / DOB        : 1
  Custom Rules Hit   : 0

  ──────────────────────────────
  TOTAL ITEMS REDACTED : 10
═══════════════════════════════════════════════
```

No actual PII data is included — only the summary counts. Store this file as part of your GDPR or HIPAA compliance documentation.

---

### 📁 Bulk File Processing

- Drag & drop `.txt` and `.csv` files directly
- Process **multiple files simultaneously**
- Per-file animated progress bar
- Per-file redaction stats (how many of each type)
- Download clean `filename_redacted.txt/.csv` output
- All processing happens locally — no upload, ever

---

### ⚙️ Custom Rules Engine

Add your own patterns specific to your firm or workflow:

| Field | Example |
|-------|---------|
| Rule Name | Employee ID |
| Pattern (regex) | `EMP-\d{5}` |
| Replace With | `[REDACTED-EMP]` |

Supports both plain keywords and full regex. Rules are applied on top of all built-in PII detection, giving you total control over what gets masked.

---

### 🕓 Session History

Every redaction action — text or file — is logged in the History tab with:
- Timestamp
- Source name (file name or text snippet)
- Per-type counts
- Total items redacted

Session history clears when you close the tab. Nothing is ever stored permanently.

---

## ⚔️ SanitizeOS vs. Cloud Tools

| | 🛡️ SanitizeOS | ☁️ Cloud Tools |
|---|:---:|:---:|
| Data stays on your device | ✅ Always | ❌ Never |
| Works without internet | ✅ Yes | ❌ No |
| No account or signup required | ✅ Yes | ❌ No |
| Zero server-side processing | ✅ Guaranteed | ❌ Core business model |
| Auditable source code | ✅ Open | ❌ Black box |
| Click-to-reveal false positives | ✅ Yes | ❌ No |
| Legal-grade masking styles | ✅ 3 styles | ⚠️ Varies |
| Downloadable compliance audit log | ✅ Yes | ⚠️ Rarely |
| Custom keyword/regex rules | ✅ Yes | ⚠️ Paid tier |
| Air-gap compatible | ✅ Yes | ❌ No |
| GDPR-safe pipeline | ✅ By design | ⚠️ Depends on ToS |
| HIPAA-safe pipeline | ✅ By design | ⚠️ Requires BAA |
| No subscription fee | ✅ $25 once | ❌ $X/month forever |
| No vendor breach risk | ✅ Zero | ❌ Real and ongoing |

---

## 📦 Free Demo vs. Paid Tool

<table>
<tr>
<td width="50%" valign="top">

### 🆓 Free Demo (`index.html`)
*This GitHub repository — no payment required*

- ✅ Live text redaction (real-time)
- ✅ Copy output to clipboard
- ✅ Detection count stats
- ✅ Sample text to test
- ❌ Masking style selection
- ❌ Click-to-reveal
- ❌ File upload / bulk processing
- ❌ Download output files
- ❌ Custom rules engine
- ❌ Audit log generation
- ❌ Session history

</td>
<td width="50%" valign="top">

### 🔓 Full Tool (`tool.html`) — $25 Lifetime
*Delivered via Gumroad — `tool.html` single file*

- ✅ Everything in free, plus:
- ✅ **3 legal masking styles**
- ✅ **Click-to-reveal** false positive fix
- ✅ **6 PII types** with per-type toggles
- ✅ **Drag & drop file uploads** (.txt, .csv)
- ✅ **Bulk multi-file processing**
- ✅ **Download redacted files**
- ✅ **Custom rules engine** (keyword + regex)
- ✅ **Compliance audit log** download
- ✅ **Session history** with counts
- ✅ Air-gap ready, works forever offline
- ✅ All future updates included

</td>
</tr>
</table>

---

## 🚀 How It Works

**Free demo — zero setup:**

```bash
git clone https://github.com/avinashwalton/sanitizeos.git
open index.html
# That's it. No npm. No build. No server.
```

**Paid tool — same simplicity:**
1. Purchase on [Gumroad](https://avinashwalton.gumroad.com/l/SanitizeOS)
2. Download `tool.html` from your Gumroad receipt email
3. Double-click it — opens in any browser, works immediately

**For air-gapped environments:**
```
1. Download tool.html on any internet-connected machine
2. Copy to USB drive
3. Transfer to air-gapped machine
4. Open in browser — zero internet needed, ever
```

**Keyboard shortcut:** `Ctrl + Enter` (or `Cmd + Enter`) triggers redaction from any tab.

---

## 🏗️ Technical Architecture

```
tool.html (Single File — ~800 lines)
│
├── HTML5 — 5-tab dashboard layout
│   └── Text Redactor · File Processor · Custom Rules · Audit · History
│
├── CSS3 — Dark glassmorphism UI
│   ├── CSS custom properties (design token system)
│   ├── Responsive grid layouts
│   └── Zero external stylesheets
│
└── Vanilla JavaScript Engine
    ├── Non-overlapping regex match collection
    ├── Priority-ordered PII detection (SSN → Card → Date → Email → IP → Phone)
    ├── Segment mapping for click-to-reveal
    ├── FileReader API (local file processing)
    ├── Blob + createObjectURL (downloads)
    ├── Custom rules engine (user-defined patterns)
    └── In-memory session history

Network Requests to Process Data:  ZERO
Third-Party SDKs with Data Access: ZERO
Cookies Set:                       ZERO
localStorage Written:              ZERO
```

---

## 💰 Pricing

<div align="center">

| Plan | Price | Masking Styles | File Processing | Audit Log | Custom Rules |
|------|-------|:-:|:-:|:-:|:-:|
| **Free Demo** | $0 | ❌ | ❌ | ❌ | ❌ |
| **Lifetime License** | **$25 once** | ✅ 3 styles | ✅ | ✅ | ✅ |

<br/>

### **[🔓 Get Lifetime Access on Gumroad — $25](https://avinashwalton.gumroad.com/l/SanitizeOS)**

*Pay once. Own it forever. No subscription. No renewal.*
*14-day no-questions-asked refund guarantee.*

</div>

---

## 💬 What Users Say

> *"The Click-to-Reveal feature alone saved me 20 minutes on a 40-page document. One regex false positive and I just clicked it — done."*
> — **James P., Paralegal, NYC**

> *"I generated the audit log and attached it to our GDPR compliance file. Our DPO was impressed — she'd never seen a tool that could prove local processing like this."*
> — **Lisa M., Data Protection Officer, London*

> *"Redacted 3,000 rows of client data from a CSV in seconds. Worth every penny for the peace of mind alone."*
> — **Priya T., CPA, Public Accounting**

---

## ❓ FAQ

<details>
<summary><strong>Does my data really never leave my device?</strong></summary>
<br/>
Yes. Open DevTools → Network tab → paste sensitive text → watch nothing fire. The JavaScript regex engine runs entirely inside your browser's local execution environment. There is no backend, no API call, no WebSocket, and no fetch() request made with your data.
<br/><br/>
</details>

<details>
<summary><strong>What are the 3 masking styles and when should I use them?</strong></summary>
<br/>
<strong>Solid Black Blocks (█████)</strong> — Mimics the classic physical redaction marker. Best for screenshots or documents that will be visually reviewed.<br/>
<strong>[REDACTED - PII]</strong> — Machine-readable, type-labelled format. Best for legal documents where the type of redacted data must be documented.<br/>
<strong>[CONFIDENTIAL]</strong> — Formal and generic. Best for internal memos and reports where you don't want to label the type.
<br/><br/>
</details>

<details>
<summary><strong>How does Click-to-Reveal work?</strong></summary>
<br/>
Each redacted block in the output pane is a clickable span element. Clicking it reveals the original underlying text (highlighted in green). Clicking again re-masks it. This is essential for handling false positives — for example, if a phone number pattern matches a non-phone number sequence in your document. Each block is independently toggleable.
<br/><br/>
</details>

<details>
<summary><strong>What exactly is in the Audit Log download?</strong></summary>
<br/>
The audit log .txt file contains: the tool name and version, a timestamp, a generated session ID, and a count of each PII type removed (e.g., "3 Emails, 1 SSN"). Crucially, it contains <strong>no actual PII data</strong> — only the summary counts. This makes it safe to store, share with compliance officers, or attach to GDPR/HIPAA documentation.
<br/><br/>
</details>

<details>
<summary><strong>Can I use custom rules alongside built-in PII detection?</strong></summary>
<br/>
Yes. Custom rules run after all built-in patterns, on the same pass. You can add plain keywords (e.g., your firm's name) or full regular expressions (e.g., case numbers like CASE-2025-\d{5}). Each custom rule has its own replacement text.
<br/><br/>
</details>

<details>
<summary><strong>Is this GDPR / HIPAA compliant?</strong></summary>
<br/>
Since data never leaves your device, SanitizeOS eliminates the cloud transmission risk that most GDPR and HIPAA guidance focuses on. The audit log provides a documented record of your redaction process. For GDPR, local processing means no third-party data processor is involved. For HIPAA, no PHI is transmitted to any covered entity or BA. Always consult your compliance officer for your specific workflow.
<br/><br/>
</details>

<details>
<summary><strong>What is the refund policy?</strong></summary>
<br/>
14-day no-questions-asked refund. If SanitizeOS doesn't work for your use case within 14 days of purchase, contact through Gumroad for a full refund.
<br/><br/>
</details>

---

## 🗺️ Roadmap

- [x] Live text redaction (6 PII types)
- [x] 3 legal masking styles
- [x] Click-to-reveal false positive fix
- [x] File upload & download (.txt, .csv)
- [x] Custom keyword / regex rules
- [x] Compliance audit log generation
- [x] Session history with per-type counts
- [ ] PDF text extraction + redaction
- [ ] Redaction audit log export (JSON format)
- [ ] Multi-file batch zip download
- [ ] International date format support (DD/MM/YYYY)
- [ ] Windows `.exe` wrapper (Electron)

> All future updates are included with the $25 lifetime license.

---

## 📜 License

This repository contains the **free demo version** (`index.html`) for evaluation.

The full licensed tool (`tool.html`) is a **commercial product** at:
👉 **[https://avinashwalton.gumroad.com/l/SanitizeOS](https://avinashwalton.gumroad.com/l/SanitizeOS)**

---

<div align="center">

**Built for professionals who take client confidentiality seriously.**

<br/>

### **[🔓 Get Lifetime Access — $25](https://avinashwalton.gumroad.com/l/SanitizeOS)**

*One file. One payment. Zero risk. 14-day refund guarantee.*

<br/>

---

Made with ❤️ in India by **[Avinash Walton](https://github.com/avinashwalton)**

*If SanitizeOS saved you from a compliance headache, consider leaving a ⭐ on GitHub.*

</div>
