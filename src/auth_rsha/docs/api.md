# API

## `AuthSettings`
Поля: `jwt_secret`, `jwt_alg="HS256"`, `access_ttl=3600`, `token_url_path="/auth/token"`.

## `make_auth_router(settings, repo)`
Регистрирует POST `${token_url_path}`. `repo` реализует протокол `UserRepository.get_by_username()`.

## `make_current_user(settings)`
Возвращает зависимость FastAPI, которая декодирует/валидирует JWT и отдаёт `TokenPayload`.

## Хеширование
`hash_password(plain)`, `verify_password(plain, hashed)` — Argon2.
