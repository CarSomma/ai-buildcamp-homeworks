# AI Buildcamp: Homework 1

Solution to Homework 1 of the AI Engineering Buildcamp. The project downloads free programming books by Allen Downey, extracts their text, and builds a RAG (Retrieval-Augmented Generation) pipeline on top of them.

## Project Structure

| File                     | Description                                                                |
| ------------------------ | -------------------------------------------------------------------------- |
| `get_books.ipynb`      | Downloads PDFs from a remote CSV into `books/`                           |
| `convert_pdf2md.ipynb` | Converts PDFs to Markdown using `markitdown`, saves to `books_text/`   |
| `rag.ipynb`            | Chunks documents, indexes with `minsearch`, and runs a full RAG pipeline |

## Setup

```bash
uv add 'markitdown[pdf]' gitsource minsearch openai
```

## Questions Covered

**Q1**: Line count of the extracted *Think Python* book
**Q2**: Number of chunks produced with `size=100, step=50`
**Q3**: Total documents indexed with `minsearch`
**Q4**: Top search result for `"python function definition"`
**Q5**: Input token count for a single RAG query
**Q6**: Structured output using a Pydantic response model
