# 🗒️ UTBM — Internship Report  

This is a template for the internship report of the UTBM. It is based on the [UTBM internship LaTeX version](https://github.com/pinam45/utbm-latex-internship-report-covers).

- 🤍 Any contribution is welcomed!

## Usage

This template has been made for and with [Visual Studio Code](https://code.visualstudio.com/), thus it may not work properly with other editors.

### Mandatory extensions

- 🚀 [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) - Used to compile the LaTeX files directly within VSCode.

### Recommended extensions

- 🔸 [LaTeX Utilities](https://marketplace.visualstudio.com/items?itemName=tecosaur.latex-utilities) - Useful extension to extends capabilities of LaTeX Workshop.
- 🪄 [LaTeX Formatter](https://marketplace.visualstudio.com/items?itemName=nickfode.latex-formatter) - Appreciate a more user friendly code base.
- 🔦 [LaTeX language support](https://marketplace.visualstudio.com/items?itemName=torn4dom4n.latex-support) - This extension adds syntax highlighting for LaTeX files.
- 📗 [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) - Don't let typos slip through the cracks.

## Requirements

There is multiple way to install LaTeX on your computer:

> **Note**  
> More information on how to install LaTeX for the LaTex Workshop extension can be found [here](https://github.com/James-Yu/LaTeX-Workshop/wiki/Install).

### Windows

#### [MikTeX](https://miktex.org/download)  

Easy to install but does not ship with Perl. If you choose MiKTeX, you have to install Perl by yourself (explained below), which the `latexmk` package requires. Without Perl, `latexmk` fails with errors.

1. You can install Perl using Strawberry Perl, which is available [here](http://strawberryperl.com/). Once it is installed, you can verify that Perl is available by opening a command prompt and typing `perl -v`. If it is installed correctly, you should see the version of Perl that you installed.

2. Verify that both Perl (this should be good if the `perl -v` command succeeded) and MiKTeX are in your `PATH`. Then if VSCode was open while you were installing them, you need to restart it.

3. After restarting VSCode, you should be able to compile your LaTeX files using the LaTeX Workshop extension!

> _Any other LaTeX distribution? Do a pull request!_

### Linux / MacOS

_I did not have the time to test it on Linux nor MacOS but any PR that would add support for these OSes would be greatly appreciated._

## Contributing

If you want to contribute to this project, feel free to make a PR 🔥
