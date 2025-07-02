# beamerthemecode

A small, minimalistic LaTeX beamer theme intended for technical presentations
where code examples are central, e.g.

- Programming talks or tutorials
- Software development demonstrations


## Code Highlighting With a Custom Pygments Style

A custom [pygments](https://pygments.org/) style is included with the theme.
This style has to be installed in an python environment of
your choice prior to building the slides. A [mamba](https://github.com/mamba-org/mamba)
environment is provided with the file `environment.yml`.
If you don't want to use the pygments style, change
the style in `headers/header.tex` or remove the `minted2`
package entirely.

## Installation

To install this theme, at least beamerthemecode.sty has to be moved to
a directory that is searchable by LaTeX. This can be one of

- `TEXMFHOME/tex/latex/beamerthemecode`. `TEXMFHOME` can be accessed via 
  ```
  $ kpsewhich --var-value TEXMFHOME
  ```
  Usually this returns `$HOME/texmf`
- The same directory you compile your document in
- Any directory which is included in `TEXINPUTS`

You can install the theme with the following command:
```
$ cd `kpsewhich --var-value TEXMFHOME` && git clone https://github.com/aknierim/beamerthemecode
```

## Acknowledgements
This theme is a LaTeX beamer adaption for a theme of a talk given by [@StFroese](https://github.com/StFroese) at the ErUM-Data-Hub PYOPP Workshop 2025.
