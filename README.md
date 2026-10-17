# C4Site open research

The research behind [c4site.com.au](https://c4site.com.au): the tool guides, where your data goes, what the rules say, the AI answers we checked, the templates and the change log. Every fact names the page it came from and the date we read it.

It's free to reuse under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Please credit "C4Site, c4site.com.au".

## What's here

| Folder | What it holds | On the site |
|---|---|---|
| `guides/` | One research file per tool guide (19 tools), every line tagged with its source, plus each connection's steps as JSON. | [AI in your tools](https://c4site.com.au/ai-in-your-tools/) |
| `data/` | Each AI assistant and plan: training, retention, storage, admin controls and human review, as JSON and CSV, with sources. | [Where your data goes](https://c4site.com.au/where-your-data-goes/) |
| `rules/` | What Australian regulators, courts, governments and education bodies have published about AI, as JSON and CSV. It reports; it isn't legal advice. | [What the rules say](https://c4site.com.au/what-the-rules-say/) |
| `it-sounded-right/` | Every question we asked local AI models, every answer word for word, the settings, the answer key with its sources, and our marks. `ask.py` reruns it. | [It sounded right](https://c4site.com.au/it-sounded-right/) |
| `templates/` | A one-page AI policy, a never-paste list, an AI tools register and lines for saying AI helped, as Word and Markdown. | [Templates](https://c4site.com.au/templates/) |
| `changes/` | When each guide was checked, and what changed in the tools since. | [What's changed](https://c4site.com.au/ai-in-your-tools/changes/) |

## Found something wrong?

Tools change, and we make mistakes. Open an issue with the page and the source that shows it, or email hello@c4site.com.au. We'll check it and fix it, and the fix goes in `changes/`.

## How it's made

The research reads each organisation's own pages: vendors' documentation, and regulators', courts' and governments' own sites. It doesn't rely on other people's blogs or summaries. What couldn't be established is published too, in each file's `gaps`. The site is built from these files, so the site and this repository say the same thing.

We use AI to help find sources and draft. Claude, Anthropic's AI, researched the answer key in `it-sounded-right/` and marked each answer against it; every mark names its source so you can check it.
