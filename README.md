# 💳 SmartCreditAI
### AI-Powered Beneficiary Credit Scoring for Inclusive Digital Lending

SmartCreditAI is a FastAPI + HTML-based credit scoring system designed for government loan beneficiaries (e.g., NBCFDC, MoSJE).  
It generates a transparent **Composite Credit Score (300–900)** using alternative data like repayment behavior, income stability, savings, and mobile usage.

---

## 🚀 Features
- 📊 Composite Credit Score (300–900)
- 🧾 Input form for beneficiary data
- ⚙️ Weighted scoring formula for repayment + income + savings
- 🎯 Risk Band Classification (Low / Medium / High)
- 💸 Recommended Loan Amounts
- 🧠 Explainable reasons behind each score
- 🗂️ SQLite database to store scores
- 🌐 API endpoint `/api/score` for JSON access

---

## ⚙️ Tech Stack
- **Backend:** FastAPI (Python)
- **Frontend:** HTML, Jinja
- **Database:** SQLite
- **Hosting:** Replit / Local / Render (demo)

---

## 🧮 Formula Used
credit_score = int(((0.4 * repayment_ratio) +
(0.3 * (income / 100000)) +
(0.2 * (savings / income)) +
(0.1 * (recharge_freq / 10))) * 900)
