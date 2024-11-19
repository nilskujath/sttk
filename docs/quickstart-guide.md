---
hide:
  - navigation
#  - toc
---

# Quickstart Guide

## Getting Started

:simple-ticktick: **Step 1**: Install `sttk` and the `notebook` package.
Then start the Jupyter Notebook server and open up a new Jupyter Notebook (`File>New>Notebook`; select `Python 3 (ipykernel)` if asked to select a kernel). 

=== ":material-language-python: pip"

    ```bash
    pip install sttk notebook
    ```

=== ":simple-poetry: poetry"

    ```bash
    poetry add sttk notebook
    ```

---

:simple-ticktick: **Step 2**: Then start the Jupyter Notebook server and open up a new Jupyter Notebook (`File>New>Notebook`; select `Python 3 (ipykernel)` if asked to select a kernel).

```bash
jupyter notebook --port=8888 # change portnumber if port is already in use
```


## Going Further...



<div class="grid cards" markdown>

-   :material-file-document-multiple:{ .lg .middle } __Read the Documentation__

    ---

    Dive into the details and understand the underlying architecture from A to Z

    [:octicons-arrow-right-24: Documentation](documentation/overview.md)

</div>