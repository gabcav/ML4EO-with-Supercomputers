# https://jameswillett.dev/getting-started-with-material-for-mkdocs/

Initial setup
pip --version
pip install mkdocs-material

Start local website
gabriele@Mac MkDocs % source venv/bin/activate                                         
(venv) gabriele@Mac MkDocs % mkdocs serve  

Generate slides in PDF
marp slides.md --pdf --allow-local-files --output custom_name.pdf


For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

I like to play :soccer:


https://squidfunk.github.io/mkdocs-material/