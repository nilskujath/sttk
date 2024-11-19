---
hide:
#  - navigation
  - toc
---

# Installation

=== ":material-language-python: pip"

    Before using this library in your projects, you may want to create a directory in which you perform your operations.
    For this tutorial, we will create and use a directory called `sttk-testdrive` and set up a dedicated virtual environment called `sttk-testenv`:

    ---

    :simple-ticktick: **Step 1**: Create a project directory.
    ```bash
    mkdir sttk-testdrive
    cd sttk-testdrive
    ```

    ---

    :simple-ticktick: **Step 2**: Create a virtual environment. 
    ```bash
    python3 -m venv ./sttk-testenv
    ```

    ---

    :simple-ticktick: **Step 3**: Activate the virtual environment.

    === "MacOS/Linux"

        ``` bash
        source sttk-testenv/bin/activate
        ```

    === "Windows"

        ```
        sttk-testenv\Scripts\activate
        ```

    ---

    :simple-ticktick: **Step 4**: Install the `sttk` library via the `pip` package installer:
    ```bash
    pip install sttk
    ```

=== ":simple-poetry: poetry"

    !!! warning "Under Construction!"

        This section is under construction!
        STTK is still a work in progress, but don’t worry—a pre-release version is just around the corner. Grab a coffee and hang tight!

---

<div class="grid cards" markdown>

-   :material-skip-next:{ .lg .middle } __Next Section__

    ---

    [:octicons-arrow-right-24: Jupyter Notebook](../../documentation/getting-started/jupyter-notebook.md)



-   :material-table-of-contents:{ .lg .middle } __Back to Documentation Overview__

    ---

    [:octicons-arrow-right-24: Documentation Overview](../../documentation/overview.md)

</div>