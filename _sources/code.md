---
jupytext:
  cell_metadata_filter: -all
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Example using Jupyter Notebook

This page is an example of using MyST Markdown to embed python code within a markdown file to add to a Jupyter Book.

## An example cell

With MyST Markdown, you can define code cells with a directive like so:

```{code-cell}
for i in range(10):
  print(i)
```

The output should be displayed in-line. 
