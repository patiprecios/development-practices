# Python Development Guidelines

This is the guide for python development

Before continue reading this guide, open a Python notebook or interactive terminal and write:

    $ python
    >>> import this
    The Zen of Python, by Tim Peters

    Beautiful is better than ugly.
    Explicit is better than implicit.
    Simple is better than complex.
    Complex is better than complicated.
    Flat is better than nested.
    Sparse is better than dense.
    Readability counts.
    Special cases aren't special enough to break the rules.
    Although practicality beats purity.
    Errors should never pass silently.
    Unless explicitly silenced.
    In the face of ambiguity, refuse the temptation to guess.
    There should be one-- and preferably only one --obvious way to do it.
    Although that way may not be obvious at first unless you're Dutch.
    Now is better than never.
    Although never is often better than *right* now.
    If the implementation is hard to explain, it's a bad idea.
    If the implementation is easy to explain, it may be a good idea.
    Namespaces are one honking great idea -- let's do more of those!

## Code style

\# TODO:

## Debugging

\# TODO:

## Code quality

Use automated tools to check code quality. Here are some examples:

- Check missing docstrings with `pydocstyle`
- Formatting/Linting checks through `flake8`
- Checks for complexity and metrics through `flake8 --max-complexity 10` or `radon`
- Typing checks through `mypy`
- Import sorting through `isort`
- Check for version changes and compatibility (check outdated).
- Audit security through `bandit`
- Audit for secrets with something like `detect-secrets` or `gitguardian`

Feel free to propose improvements and changes.

## Testing & coverage

Use standard testing and coverage tools.

We strongly encourage that all the code you write be tested. You can use frameworks like `pytests`, `hypothesis` and `coverage`.

## Python versions

Preferably use the latest stable release of python. Migrate periodically, don't let the code gets old.

## Dependency management

Use standard tools for dependency management like `pip` or `conda`. Options may be allowed if the tool is stable.

Periodically check outdated libraries.

    pip list -o
