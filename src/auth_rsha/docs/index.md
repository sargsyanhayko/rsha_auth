# auth-rsha

JWT аутентификация для FastAPI (password flow).  
`pip install auth-rsha`

- `/auth/token` — выдаёт access-токен по `username/password`
- `make_current_user()` — зависимость, валидирующая Bearer JWT
- Хеш пароля: `argon2`

→ см. **Getting started**
