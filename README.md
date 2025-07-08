# P2P Scam Verification Checklist

This guide provides a structured approach to identifying and mitigating fraud risks in peer-to-peer (P2P) cryptocurrency trading environments. It has been developed through practical experience in high-volume OTC and informal P2P groups, primarily in Russian-speaking crypto communities.

## Overview
Fraud in P2P crypto trading is often perpetrated through fake payment screenshots, chargebacks, forged confirmations, and deceptive identification practices. This checklist is designed to help traders and compliance analysts verify transaction authenticity before releasing crypto assets.

---

## 1. EXIF Data Checks
Fraudsters often send doctored images as "proof" of payment. These may include manipulated timestamps, overlays, or template screenshots reused across multiple scams.

### ✅ How to check:
- **Inspect image metadata (EXIF)** using Telegram bots or EXIF readers.
- Look for camera model inconsistencies or missing metadata (sign of editing).
- Check creation vs modification timestamps — if they're mismatched or too recent, it's likely edited.

### 🔍 Example:
A user claimed to send a transfer at 14:38. EXIF data revealed image creation time as 14:41 — after they demanded the release of crypto.

---

## 2. QR Code Structure Analysis
Scammers may send QR codes that appear to be payment confirmations, but are actually generic or reused images.

### ✅ How to check:
- Decode the QR with a scanner bot or phone — verify if it contains actual transaction details.
- Check for consistency: bank name, amount, transaction ID.
- Look for signs of screenshot cropping or template reuse.

### 🔍 Example:
QR led to a static PNG hosted online — not linked to a real transaction.

---

## 3. Bank Statement Comparison
Scammers might send PDF/PNG “statements” showing that payment was made.

### ✅ How to check:
- Confirm the **sender name matches the verified identity**.
- Compare the **bank interface UI** to known real ones (scammers often use templates).
- Validate presence of **transaction number**, not just “sent” message.

### 🧠 Tip:
Request delayed screenshots (10 minutes later) — scammers often can’t reproduce a time-consistent fake.

---

## 4. Risk Factor Scoring
Use a scoring system to determine release risk. Each inconsistency or red flag increases the threshold.

### Sample factors:
- ⛔ No EXIF data → +1 risk
- ⛔ QR code generic → +2 risk
- ⛔ Timestamp mismatch → +3 risk
- ⛔ Unverified sender name → +2 risk

If total score >5 → delay transaction, request video proof or decline.

---

## ✅ Outcome
This checklist was applied in 50+ real-world investigations and resulted in prevention of over $2,000 in potential losses. It is now adopted by multiple OTC/P2P communities for day-to-day verification.

---