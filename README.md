# K-9 Mail User Manual

This repository is the home of the user documentation for [K-9 Mail](https://k9mail.app/). Contributions are welcome.

Uses [mkdocs](https://www.mkdocs.org/) to generate static HTML.

Changes to the `main` and `stable` branch are automatically published to the website using GitHub Actions.

The `main` branch contains the documentation for the current beta version.

The `stable` branch contains the documentation for the current stable version and is displayed by default when the site is accessed via <https://docs.k9mail.app/>.

## Install dependencies

Best is using a virtual environment to avoid conflicts with other Python projects:

```shell
python -m venv venv
```

Activate the virtual environment. You need to do this every time you want to build the site:

```shell
source virtual_env/bin/activate
```

Install the dependencies:

```shell
pip install -r requirements.txt
```

After you are done, deactivate the virtual environment:

```shell
deactivate
```

## Building the Site

To preview local changes, run

```shell
mkdocs serve --config-file config/en/mkdocs.yml
```

then visit <http://127.0.0.1:8000/en/>.

## Creating Screenshots

We automated the creation of screenshots. The tools and a short explanation can be found in the [user-manual](https://github.com/thundernest/k-9/tree/main/user-manual) directory of the [K-9 Mail app repository](https://github.com/thundernest/k-9).
