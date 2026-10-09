# Academic CV

`Sun_Wei_Academic_CV_LaTeX.tex` is the editable source for the two-page academic CV.
`Sun_Wei_Academic_CV.pdf` is the downloadable copy; keep it identical to
`assets/sun-wei-academic-cv.pdf` inside `website.zip` when updating the CV.
Compile twice with XeLaTeX and the TeX Gyre Pagella/Heros fonts. For example,
from this directory, using a separate build directory:

```sh
mkdir -p /tmp/sun-wei-cv-build
xelatex -interaction=nonstopmode -halt-on-error -output-directory=/tmp/sun-wei-cv-build Sun_Wei_Academic_CV_LaTeX.tex
xelatex -interaction=nonstopmode -halt-on-error -output-directory=/tmp/sun-wei-cv-build Sun_Wei_Academic_CV_LaTeX.tex
```

After checking both rendered pages, replace `assets/sun-wei-academic-cv.pdf`
inside the repository's `website.zip` with the compiled PDF. The Pages workflow
deploys the ZIP contents; changing an extracted local copy alone does not update
the website. The Chinese portfolio PDF is a separate, unchanged document.
