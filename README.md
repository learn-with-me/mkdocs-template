# MkDocs Template

Template for documenting my notes

## Installation

To begin working on this run the following: 

```
$ pip install mkdocs mkdocs-bootstrap
```

Then `cd` into this directory and run: 

```
$ mkdocs serve
```

This will open a browser session in [http://localhost:8000](http://localhost:8000) where you can add, edit, or delete documentation in live mode.

## Building the Site

```
$ mkdocs build --clean
```
The `site` directory will then contain the code.

## Hosting the Site

### Deploying to GitHub Pages

```
$ mkdocs gh-deploy
```

### Deploying to S3

Alternatively, the documentation can also be hosted in S3. We can upload the `site` directory to S3 with:

```
$ aws s3 cp site s3://docs.goel4ever.com --recursive --acl public-read
```

### Create new project instead

Instead of using the template as base, to start from scratch, use the following command

```
$ mkdocs new my-project
```

## References

- MkDocs [official site](https://www.mkdocs.org/getting-started/)
- [Choosing your theme](https://www.mkdocs.org/user-guide/choosing-your-theme/)
  - [Third-party themes](https://github.com/mkdocs/mkdocs/wiki/MkDocs-Themes)
    - [MkDocs Material](https://squidfunk.github.io/mkdocs-material/getting-started/)
    - [Alternatives](https://squidfunk.github.io/mkdocs-material/alternatives/)
  - [Additional third-party themes](https://www.wheelodex.org/entry-points/mkdocs.themes/)
- [Deploying the docs](https://www.mkdocs.org/user-guide/deploying-your-docs/)
