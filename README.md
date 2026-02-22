# LLM-Powered Entity Extraction from Documents

Extracting entities from legal documents with LLMs

## Installation

```bash
# Clone the repository
git clone https://github.com/gafnts/llm-entity-extractor.git
cd llm-entity-extractor

# Install dependencies
uv sync
```

## Development Setup

```bash
# Install with development dependencies
uv sync --dev

# Install pre-commit hooks
uv run pre-commit install
```

## Usage

```bash
# Run the tool
uv run llm-entity-extractor
```

## Development

### Linting and Formatting

```bash
# Run all pre-commit checks
uv run pre-commit run --all-files

# Or run individual tools:

# Check linting
uv run ruff check .

# Auto-fix linting issues
uv run ruff check --fix .

# Check formatting
uv run ruff format --check .

# Apply formatting
uv run ruff format .
```

### Type Checking

```bash
# Run mypy
uv run mypy src/
```

### Adding Dependencies

```bash
# Add a runtime dependency
uv add package-name

# Add a development dependency
uv add --dev package-name
```

## CI

This project uses GitHub Actions for continuous integration. On every PR to main, the workflow:
- Runs ruff linting and formatting checks
- Runs mypy type checking
- Executes all pre-commit hooks

## License

See [LICENSE](LICENSE) for details.
