# Getting started

`auth-rsha` — это готовый JWT-модуль для FastAPI по password-flow.
- Выдаёт access-токен по `username/password`
- Даёт зависимость `make_current_user()` для проверки Bearer-JWT
- Пароли — Argon2 (`hash_password/verify_password`)
- Настройки берутся из Pydantic Settings (ENV или `.env`)

## Установка

```bash
pip install auth-rsha
