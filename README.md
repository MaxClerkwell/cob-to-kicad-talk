# CoB to KiCad Integration

Slides: *From Bare Die to Bonded Board: Chip-on-Board Meets KiCad*.
LaTeX Beamer, 16:9.

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

## License

The slides, the LaTeX source and the images made for this talk are licensed under the
[Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/)
(CC BY 4.0). See [`LICENSE`](LICENSE).

You may copy, modify, share and use them commercially, as long as you credit the work and
indicate if you changed it. Suggested attribution:

> From Bare Die to Bonded Board: Chip-on-Board Meets KiCad, by Stephan Bökelmann,
> https://github.com/MaxClerkwell/cob-to-kicad-talk, licensed under CC BY 4.0.

Not covered by this license: the Xiaohongshu logo (`images/xiaohongshu.*`) and the
CERN lettering visible in the photo belong to their owners.
Images taken from [open.cob.json](https://github.com/MaxClerkwell/open.cob.json) are also CC BY 4.0.
