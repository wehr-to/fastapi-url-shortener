# fastapi-url-shortener

A secure, FastAPI-based URL shortening service. Built to demonstrate redirect logic, link expiration, and safe link validation — while simulating common security pitfalls in open redirect flows.

## 🛠️ Learning Goals

- Build a URL shortener with redirect logic
- Store original and short links in a database
- Prevent common open redirect vulnerabilities
- Apply input validation and expiration handling

## 🔐 Security Focus

This app includes protections against:

- ✅ Open Redirects
- ✅ Unsafe or unvalidated URLs
- ✅ Excessively long or malformed inputs
- ✅ Shortlinks pointing to malicious domains (optional)

See [`audit-checklist.md`](./audit-checklist.md) for a full breakdown.

## 📦 Features

- Create custom or auto-generated shortlinks
- Redirect with FastAPI routing
- SQLite/PostgreSQL support via SQLAlchemy or Tortoise
- Input validation (e.g. regex, domain checks)
- Optional link expiration dates
- Optional integration with Safe Browsing APIs

## 🤝 Contributions
Pull requests are welcome! If you’d like to add features, improve security hardening, optimize code, or extend functionality, feel free to open an issue or PR. This is a learning-focused lab project, and collaboration is encouraged.

## 🚀 Getting Started

```bash
git clone https://github.com/yourusername/fastapi-url-shortener.git
cd fastapi-url-shortener
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
uvicorn app.main:app --reload

🔒 Bonus Features
✅ Link expiration support (expires_at)
✅ Redirect validation using regex or API
✅ Markdown doc rendering with OpenAPI/Swagger
✅ Logging and audit records



