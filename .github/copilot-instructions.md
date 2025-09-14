# Copilot Instructions for AI Coding Agents

## Project Overview
- This repository is a community-curated list of public APIs, managed via the main `README.md` file.
- Validation and testing scripts are located in `scripts/`, with Python-based checks for format and link integrity.
- The project is maintained by contributions and pull requests, with automated validation workflows.

## Key Components
- `README.md`: The central data file listing APIs. All additions/edits should follow its formatting conventions.
- `scripts/validate/format.py`: Validates the format of `README.md`. Run with `python scripts/validate/format.py README.md`.
- `scripts/validate/links.py`: Validates links in `README.md`. Run with `python scripts/validate/links.py README.md`.
- `scripts/requirements.txt`: Python dependencies for validation scripts.
- `scripts/tests/`: Contains unit tests for validation logic.
- `.github/workflows/`: Contains GitHub Actions for CI validation (`validate_links.yml`, etc.).

## Developer Workflows
- **Validation**: Always validate changes to `README.md` using both format and link scripts before submitting PRs.
- **Testing**: Run unit tests in `scripts/tests/` to verify validation logic. Use standard Python test runners.
- **Dependencies**: Install with `python -m pip install -r scripts/requirements.txt`.
- **CI/CD**: GitHub Actions automatically run validation on PRs and pushes.

## Conventions & Patterns
- All API entries in `README.md` must follow the established table format and category structure.
- Validation scripts expect the file to be in the root and named `README.md`.
- Python scripts in `scripts/validate/` are the source of truth for validation logic.
- No external database or backend; all data is in markdown.

## Integration Points
- External dependencies are managed via `scripts/requirements.txt`.
- No direct API calls or dynamic data fetching; all updates are manual and validated locally and via CI.

## Examples
- To validate format: `python scripts/validate/format.py README.md`
- To validate links: `python scripts/validate/links.py README.md`
- To install dependencies: `python -m pip install -r scripts/requirements.txt`

## References
- See `scripts/README.md` for more details on validation and testing.
- See `.github/workflows/` for CI configuration.
- See `CONTRIBUTING.md` for contribution guidelines.

---

**If any section is unclear or missing important project-specific details, please provide feedback for further refinement.**
