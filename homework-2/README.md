# AI Buildcamp: Homework 2

Solution to Homework 2 of the AI Engineering Buildcamp. The project builds a Wikipedia-powered agent that searches for pages and fetches their content to answer questions.

## Project Structure

| File                            | Description                                                                 |
| ------------------------------- | --------------------------------------------------------------------------- |
| `wiki_tools.ipynb`              | Calls the Wikipedia Search and Get Page APIs and defines reusable functions |
| `agent_setup.ipynb`             | Sets up an OpenAI agent with tool schemas and traces a single tool call     |
| `agentic-tool-call-loop.ipynb`  | Implements a `while True` loop that drives the agent until no tools remain  |

## Setup

```bash
uv add openai requests
```

## Questions Covered

**Q1**: Total results returned by the Wikipedia Search API for `"capybara"`
**Q2**: Number of result titles containing the word *capybara* (case-insensitive)
**Q3**: Character count of the raw *Capybara* Wikipedia page
**Q4**: Agent setup with `search_wikipedia` and `get_page` tools
**Q5**: Agent answer for `"What is this page about? https://en.wikipedia.org/wiki/Capybara"`
**Q6**: Total tool calls made by the agent when asked about threats to capybara populations
