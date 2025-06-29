# Bayesian Experimentation

A practical guide to Bayesian experimentation using Quarto.

Focus:
- Intuitive examples and explanations
- Hands-on simulations
- Pragmatic approach to real-world problems

Currently a collection of posts that may evolve into a comprehensive book.

Contributions welcome.

## Quick Start

Preview book with live reload:

```bash
quarto preview
```

Build the book:

```bash
quarto render
```

## Project Structure

- `*.qmd` - Book chapters
- `_quarto.yml` - Book configuration
- `_book/` - Generated HTML output

## Development

### Environment Setup

#### Installing Quarto

This project requires [Quarto](https://quarto.org/) to build and preview the book.

#### Installing uv

This project uses [uv](https://github.com/astral-sh/uv) for Python dependency management.  

### Virtual Environment

The project uses Python 3.12. To set up the virtual environment with relevant packages:

```bash
uv sync
```

### Managing Dependencies

```bash
# Add a new dependency
uv add package-name

# Add a development dependency
uv add --dev package-name

# Update dependencies
uv sync --upgrade

# Remove a dependency
uv remove package-name
```

### Working with the Book

Add new chapters by creating `.qmd` files and updating `_quarto.yml`. Include executable code blocks for examples.

```bash
quarto preview
```

To render the book (do it before opening a merge request):

```bash
quarto render
````



