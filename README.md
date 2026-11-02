# CoB to KiCad Integration

Slides: *Understanding and solving the challenges of accelerated chip fabrication*.
LaTeX Beamer, 16:9. Work in progress, first iteration.

## Build

Needs `pdflatex`, `latexmk` and the usual TeX Live packages (beamer, tikz, qrcode, fontawesome5).

```bash
make          # build slides.pdf
make watch    # rebuild on every change
make clean    # remove build/
```

## Release

Pushing a tag that starts with `v` builds the slides in GitHub Actions and attaches
the PDF to a GitHub release:

```bash
git tag v0.1.0
git push origin v0.1.0
```

Pushes to `main` and pull requests only build the PDF and upload it as a workflow artifact.

## TODO

- Add `images/portrait.jpg` for the about-me slide (a placeholder is shown until then).
- Images in `images/` come from [open.cob.json](https://github.com/MaxClerkwell/open.cob.json) (CC BY 4.0).
