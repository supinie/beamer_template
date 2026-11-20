# beamer_template

My own version of the official Imperial College London Beamer template, which I use as the starting point for presentations.
It is not the official template; the original README follows below.

## Differences from the standard version

- Maths is set in serif (`\usefonttheme[onlymath]{serif}`) with the newtx (Times) fonts; slide text stays in Imperial Sans.
- Extra packages: soul (strikethrough), multicol, algorithm/algpseudocode and wrapfig.
- biblatex (BibTeX backend, `alphabetic` style) for citations.
- The theme files (`beamer*themeImperial.sty`) are unchanged; all changes are in the preamble of `template_presentation.tex`.
- `shell.nix` and `.envrc` provide TeX Live through Nix and direnv; build with `latexmk -xelatex template_presentation.tex`.

## Bibliography

The bibliography is the shared [`supinie/bibliography`](https://github.com/supinie/bibliography) repository, included as the submodule `bibliography/`, with [cryptobib](https://cryptobib.di.ens.fr/) nested inside it.
Clone with `git clone --recursive`.
A daily GitHub Action keeps this template's submodule on the latest commit of `bibliography`; it only runs in the template repositories, so projects created from this template keep their pinned bibliography until updated by hand with `git submodule update --remote --recursive bibliography`.

## Original README

This is the official Beamer template for Imperial
College London. Letter and poster templates are also available.

### Issues

Please report any bugs in the templates on GitHub (https://github.com/ImperialCollegeLondon/imperial_latex_templates/issues).

### Copyright

© Imperial College London, 2024. These templates, including logo and fonts, are 
for use of Imperial staff and students only for university business. All rights 
reserved to the copyright owners.
