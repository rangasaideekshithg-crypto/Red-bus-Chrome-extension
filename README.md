# RedBus Smart Assistant

Chrome extension with live RedBus listing extraction, bus comparison and
recommendations, an OpenRouter-backed travel assistant, fare history/alerts,
and optional browser voice controls.

Start with [the setup guide](docs/setup.md) and see the
[architecture overview](docs/architecture.md). The backend uses SQLite by
default; configure `DATABASE_URL` for MySQL. Never put provider keys in the
extension or commit `backend/.env`.

The supplied `backend/data/redbus_sample_buses_DEMO.csv` is exposed as a
65-route picker in the side panel. Its 520 bus rows are explicitly sample data;
the CSV is not used as live inventory, fare quotes, or seat availability.
Current bus results are extracted only from the selected RedBus route page.