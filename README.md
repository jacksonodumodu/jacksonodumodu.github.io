# jacksonodumodu.github.io

My introduction and my blog. Two computational posts analyse the Palmer Penguins data, one in R and one in Python. The site is built into `docs/`, which GitHub Pages publishes.

## Install first

- Git 2.55.0
- Quarto 1.10.18
- uv 0.12.5
- R 4.6.1

## Build

Run everything from the repository root.

In a terminal:

```
git clone git@github.com:jacksonodumodu/jacksonodumodu.github.io.git
cd jacksonodumodu.github.io
uv sync
```

In an R console opened in this folder:

```r
renv::restore()
```

Back in the terminal:

```
uv run quarto render
```

## Output

The site is written to `docs/`. Open `docs/blog.html`, or see the published version at https://jacksonodumodu.github.io.

## Data

[Palmer Penguins](https://allisonhorst.github.io/palmerpenguins/) (Palmer Station Antarctica LTER, CC0). It ships inside the `palmerpenguins` R and Python packages, so no data file is committed. Rendering needs no network. Only `uv sync` and `renv::restore()` do, to download packages.
