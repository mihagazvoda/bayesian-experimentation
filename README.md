# Bayesian Experimentation

A practical guide to Bayesian experimentation using Quarto.

Focus:
- Intuitive examples and explanations
- Hands-on simulations
- Pragmatic approach to real-world problems

Currently a collection of posts that may evolve into a comprehensive book.

Contributions welcome.

## Project Structure

- `*.qmd` or `*.ipynb` - Book chapters
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

Add new chapters by creating `.qmd` or `.ipynb` files and updating `_quarto.yml`. 

To render (or preview) only your file, use: 

```bash
uv run quarto render filename.qmd
```

```bash
uv run quarto preview filename.qmd
```

For the whole book:

```bash
uv run quarto preview
```

or

```bash
uv run quarto render
```



### If you prefer notebooks

You can work in Jupyter Notebook / Lab and then [convert the file to quarto](https://quarto.org/docs/tools/jupyter-lab.html#converting-notebooks):

```bash
uv run quarto convert basics-jupyter.ipynb # converts to qmd
uv run quarto convert basics-jupyter.qmd   # converts to ipynb
```
