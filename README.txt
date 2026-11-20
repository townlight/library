  Parked foundation — outside the released Windows suite. This repository contains exploratory/support code, not a completed Townlight product. It is not installed or supported by Windows 1.8.1.1. Historical examples, package names and dependency pins below describe this foundation and must not be used as current suite installation instructions. Use the released Windows suite, current modules and acceptance limits.

Townlight Library

Townlight Library v0.1.1 ships the municipal library support foundation for Townlight: cited library policy Q&A, program and event Q&A, optional database-backed program/collection workpapers, reference assistance over collection metadata, collection development guidance, FastAPI runtime, public sample UI, docs, tests, browser QA, and release gates.

It is not an integrated library system, patron-record access path, circulation workflow, holds or fines system, replacement for professional reference service, live LLM runtime, or library connector.

Install:

    python -m pip install -e ".[dev]"
    python -m uvicorn civiclibrary.main:app --host 127.0.0.1 --port 8143

Townlight Library v0.1.1 is pinned to civiccore==0.3.0.

Set CIVICLIBRARY_WORKPAPER_DB_URL to persist program answers and collection guidance. Without it, Townlight Library remains deterministic and stateless.

License

Code: AGPL-3.0-only, with the TownLight Public Institution Exception for qualifying deployments. See LICENSE and LICENSE-EXCEPTION.md. Documentation: CC BY 4.0 (LICENSE-DOCS).
