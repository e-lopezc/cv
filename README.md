# CV

I keep my CV in Markdown ([`cv-eliaslopez.md`](cv-eliaslopez.md)) and let GitHub Actions turn it into a PDF, so I only ever edit one file.

## Updating it

Edit the Markdown and open a PR into `current`. The workflow in [`.github/workflows/update_cv.yaml`](.github/workflows/update_cv.yaml) runs Pandoc with XeLaTeX, rebuilds `cv-eliaslopez.pdf`, and commits it back to the branch. No need to touch the PDF yourself.

## Building it locally

If you want to preview the PDF without a PR, install Pandoc and a LaTeX distribution with `xelatex`, then run:

```bash
pandoc cv-eliaslopez.md \
  --pdf-engine=xelatex \
  --variable mainfont="Latin Modern Roman" \
  --variable fontsize=11pt \
  --variable geometry="margin=1in" \
  --variable colorlinks=true \
  -o cv-eliaslopez.pdf
```
