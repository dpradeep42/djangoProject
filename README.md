# DjangoBasic

A small Django practice project. `/` returns a plain "Hello World!" response, and `/admin/` is Django's admin site.

## Setup

Python 3.10 or newer.

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
cp .env.example .env
```

Edit `.env` and set `SECRET_KEY` to a long random string. From `DjangoBasic/`:

```bash
python manage.py migrate
python manage.py runserver
```

The site listens on http://127.0.0.1:8000/.

## Environment variables

`DjangoBasic/DjangoBasic/settings.py` reads these from the environment. If a variable is missing, a `.env` file next to `manage.py` is used, then a `.env` file at the repository root. Variables already set in the environment are left unchanged.

| Variable | Default | Purpose |
| --- | --- | --- |
| `SECRET_KEY` | `dev-only-insecure-key` | Signing key. Replace it before any shared or production use. |
| `DEBUG` | `False` | Debug mode when the value is `True`, `1`, `yes`, or `on`. Anything else, including an unset variable, leaves it off. |
| `ALLOWED_HOSTS` | empty | Comma-separated hostnames, for example `localhost,127.0.0.1`. Required when `DEBUG` is off. |

Do not commit `.env`.

## License

Released under the MIT License. See [LICENSE](LICENSE).
