# 🗒️ UTBM — Internship Report  

<!-- badges  -->
![Contribute](https://img.shields.io/badge/Contribute%20!-C9284D?style=for-the-badge)
![GitHub](https://img.shields.io/github/license/Juknum/UTBM-Internship-Report?style=for-the-badge)
![GitHub last commit](https://img.shields.io/github/last-commit/Juknum/UTBM-Internship-Report?style=for-the-badge)

This repository is a Visual Studio Code template for internship reports at the UTBM. It is based on the [UTBM internship LaTeX version](https://github.com/pinam45/utbm-latex-internship-report-covers).

## I. Usage

> **Warning**  
> This template is free to use, but the covers belongs to the [UTBM](https://www.utbm.fr/) and can only be used with their authorization.

> **Note**  
> UTBM and all UTBM-related trademarks and logos are trademarks or registered trademarks of the [University of Technology of Belfort-Montbéliard](https://www.utbm.fr/) in France, other countries, or both.

This template has been made for and with [Visual Studio Code](https://code.visualstudio.com/), thus it may not work properly with other editors.

### 1. Mandatory extensions

- 🚀 [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) - Used to compile the LaTeX files directly within VSCode.

### 2. Recommended extensions

- 🔸 [LaTeX Utilities](https://marketplace.visualstudio.com/items?itemName=tecosaur.latex-utilities) - Useful extension to extends capabilities of LaTeX Workshop.
- 🪄 [LaTeX Formatter](https://marketplace.visualstudio.com/items?itemName=nickfode.latex-formatter) - Appreciate a more user friendly code base.
- 🔦 [LaTeX language support](https://marketplace.visualstudio.com/items?itemName=torn4dom4n.latex-support) - This extension adds syntax highlighting for LaTeX files.
- 📗 [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) - Don't let typos slip through the cracks.

### 3. UTBM's Covers

You can find all configurable options of UTBM covers within the below code, but if you feel unhappy you can still edit the covers [with this file here](https://github.com/Juknum/UTBM-Internship-Report/blob/main/libs/utbmcovers/utbmcovers.sty).  
<!-- Code block mention (GitHub markdown feature) -->
https://github.com/Juknum/UTBM-Internship-Report/blob/019a0ab83cf017845094d0e7b5cbc7269b072c82/main.tex#L7-L48

You can also modify colors using those variables:  
https://github.com/Juknum/UTBM-Internship-Report/blob/019a0ab83cf017845094d0e7b5cbc7269b072c82/libs/utbmcovers/utbmcovers.sty#L36-L55

Finally you can call both covers using:

```tex
\makeutbmfrontcover{} % Front cover
\makeutbmbackcover{}  % & Back cover
```

Covers support english and french languages, you can change the language using the `babel` package:

```tex
\usepackage[english]{babel} % English
\usepackage[french]{babel}  % French
```

### 4. Compile

To compile the report, you can use the <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>B</kbd> shortcut or the `LaTeX Workshop: Build LaTeX project` command inside Visual Studio Code.

## II. Requirements

This template requires the following software/packages to be installed:

- [LaTeX](https://www.latex-project.org/get/)
- The Tahoma font as the original covers are using it.

There is multiple way to install LaTeX on your computer:

> **Note**  
> More information on how to install LaTeX for the LaTex Workshop extension can be found [here](https://github.com/James-Yu/LaTeX-Workshop/wiki/Install).

### 🪟 Windows

#### [MikTeX](https://miktex.org/download)  

Easy to install but does not ship with Perl. If you choose MiKTeX, you have to install Perl by yourself (explained below), which the `latexmk` package requires. Without Perl, `latexmk` fails with errors.

1. You can install Perl using Strawberry Perl, which is available [here](http://strawberryperl.com/). Once it is installed, you can verify that Perl is available by opening a command prompt and typing `perl -v`. If it is installed correctly, you should see the version of Perl that you installed.

2. Verify that both Perl (this should be good if the `perl -v` command succeeded) and MiKTeX are in your `PATH`. Then if VSCode was open while you were installing them, you need to restart it.

3. After restarting VSCode, you should be able to compile your LaTeX files using the LaTeX Workshop extension!

> _Any other LaTeX distribution? Do a pull request!_

### 🖥️ Linux / MacOS

> _I did not have the time to test it on Linux nor MacOS but any PR that would add support for these OSes would be greatly appreciated._

## III. Contributing

If you want to contribute to this project, feel free to make a PR 🤍
