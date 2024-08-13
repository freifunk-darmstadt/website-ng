# Freifunk Darmstadt Website

After the long and tedious years we've put up with the old Jekyll website,
it was decided to rewrite the website in ~~rust~~ python.

The website is built using [mkdocs](https://www.mkdocs.org/) and the
[material theme](https://squidfunk.github.io/mkdocs-material/).

Every page is written in markdown. A quick-start on how to write
a page for mkdocs can be found [here](https://www.mkdocs.org/user-guide/writing-your-docs/).

The framework allows you to use various markdown extendions which are documented
[here](https://squidfunk.github.io/mkdocs-material/reference/).

## Development

You can spawn a local development server by running `mkdocs serve` in the root directory
of this repository.

To run this in a docker container with the same environment as the CI/CD pipeline, you
can use the following command:

```bash
docker run -it --rm --volume $(pwd):/docs ghcr.io/squidfunk/mkdocs-material:9.5.18 serve
```

Make sure you are in the root directory of this repository when running this command.
