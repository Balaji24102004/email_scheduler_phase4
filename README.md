
# Phase 4: Email Delivery using SMTP

## 📌 Objective
This phase implements the functionality to deliver dynamically generated emails via SMTP (Gmail server). The system ensures that each email in the campaign series is delivered to the intended recipients without duplication.

---

## 🛠️ Technologies Used
- **Python 3.x**
- `smtplib` — for sending emails
- `email.message` — to structure the email (subject, body, CTA)
- `dotenv` — for securely loading SMTP credentials from `.env`
- **Gmail SMTP Server** (smtp.gmail.com)

---

## 📂 Files Used in Phase 4

| File Name            | Purpose                                             |
|---------------------|-----------------------------------------------------|
| `scheduled_email.py` | Main script: Generates and sends emails via SMTP    |
| `campaign.json`      | Stores campaign details like email series and recipients |
| `campaign_state.json`| Tracks which emails have already been sent to avoid duplication |
| `campaign_parser.py` | Manages state loading and updating of `campaign_state.json` |
| `campaign_state.py`  | Loads campaign configuration from JSON file         |
| `.env`              | Stores email credentials (Not to be uploaded to GitHub) |
| `test_gemini.py`    | Optional: Tests Google Gemini API connection and response |

---

## ⚙️ Setup Instructions for Phase 4

1. **Install required libraries:**

```bash
pip install schedule python-dotenv google-generativeai
