<h1>
  <picture>
    <source
     srcset="https://github.com/Juknum/Juknum/assets/49886317/11f7f0ad-b50f-4a6b-8aec-422bacedd62e"
     media="(prefers-color-scheme: dark)" />
    <source
     srcset="https://github.com/Juknum/UTBM-Internship-Report/assets/49886317/71a5ae6f-f7aa-465a-a1a6-83975aa35adc"
     media="(prefers-color-scheme: light), (prefers-color-scheme: no-preference)" />
    <img height="24" src="https://github.com/Juknum/UTBM-Internship-Report/assets/49886317/71a5ae6f-f7aa-465a-a1a6-83975aa35adc" />
   </picture>
  UTBM — Internship Report Template
</h1>

<!-- badges  -->
![GitHub](https://img.shields.io/github/license/Juknum/UTBM-Internship-Report?style=for-the-badge)
![GitHub last commit](https://img.shields.io/github/last-commit/Juknum/UTBM-Internship-Report?style=for-the-badge)

<p>
This repository serves as a template for internship reports at UTBM. It is built upon the <a href="https://github.com/pinam45/utbm-latex-internship-report-covers">UTBM internship LaTeX version</a> and has been updated, adapted and expanded with multiple functionalities.
</p>

## I. Support

This template can be used in several places:

- Online with [Overleaf](https://www.overleaf.com) or GitHub Codespaces
- Locally on Windows/MacOS/Linux

---

## II. Features

> [!IMPORTANT]  
> This template is free to use, but the covers belongs to [UTBM](https://www.utbm.fr/) and can only be used with their authorization.  

> [!NOTE]  
> UTBM and all UTBM-related trademarks and logos are trademarks or registered trademarks of the [University of Technology of Belfort-Montbéliard](https://www.utbm.fr/) in France, other countries, or both.

### UTBM's Covers

You can find all configurable options for UTBM covers in the code below. If you're unsatisfied, you still have the option to edit the covers using [this file](https://github.com/Juknum/UTBM-Internship-Report/blob/main/libs/utbmcovers.sty).  
<!-- Code block mention (GitHub markdown feature) -->

https://github.com/Juknum/UTBM-Internship-Report/blob/108d23dee1516941a37bd0aa2fcbf109c8e18f6c/main.tex#L32-L55  

You can also modify their colors using these variables:  
<!-- Code block mention (GitHub markdown feature) -->

https://github.com/Juknum/UTBM-Internship-Report/blob/108d23dee1516941a37bd0aa2fcbf109c8e18f6c/libs/utbmcovers.sty#L36-L55  

Finally you can call both covers using:

```tex
\makeutbmfrontcover{} % Front cover
\makeutbmbackcover{}  % & Back cover
```

Covers support English and French languages, you can change the language using the `babel` package:

```tex
\usepackage[english]{babel} % English
\usepackage[french]{babel}  % French
```

---

## III. Usage

There are multiple ways to use this template; you can either use it online or locally:

### Online

<table>
  <tr>
    <th>
      <img src="https://cdn.overleaf.com/img/ol-brand/overleaf_og_logo.png" height="16" style="margin: 0 3px -2px 0;">
      Overleaf
    </th>
  </tr>
  <tr>
    <td>

1. There are two ways to import this template on [Overleaf](https://www.overleaf.com/):
    - You can either use the "Import from GitHub" button and paste the link of this repository. (This method requires a paid plan)
    - Alternatively, you can download the repository as a zip file and upload it on Overleaf. (This method is free)

2. The last step is to change the compiler from `pdfLaTeX` to `XeLaTeX`. You can do this by clicking on the `Menu` button and finding it in the `Settings` category.

    </td>
  </tr>
</table>

<table>
  <tr>
    <th>
      <img src="https://github.com/Juknum/UTBM-Internship-Report/assets/49886317/dba03968-0b1a-4812-a82d-742ffc8c31a8"  height="16" style="margin: 0 6px -2px 0;">
      GitHub Codespaces
    </th>
  </tr>
  <tr>
    <td>

1. Use this repository as a template by clicking on the `Use this template` button or by clicking [here](https://github.com/new?template_name=UTBM-Internship-Report&template_owner=Juknum).
2. Once you have your own repository, open it as a GitHub Codespaces and wait for it to fully build.
3. Install the recommended VSCode extension to be able to compile your files with [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop)
4. Run the following command to get full git access:

  ```bash
    git config --global --add safe.directory /workspace
  ```

</td>
</tr>
</table>

<p align="center"><i>Any other online LaTeX editors to suggest?</i><p>

### Locally

Use this repository as a template by clicking on the `Use this template` button or by clicking [here](https://github.com/new?template_name=UTBM-Internship-Report&template_owner=Juknum).

#### Part A: LaTeX distribution

You will need a LaTeX distribution to compile this project locally. Here is a list of tested and working distributions for this project:

<table>
<tr>
<th>
  <img src="https://github.com/Juknum/UTBM-Internship-Report/assets/49886317/2162967b-c3ff-4c70-94cd-ce5a31156814"  height="16" style="margin: 0 6px -2px 0;">
  MiKTeX
</th>
</tr>
<tr>
<td>
<a href="https://miktex.org/download">Website</a> — <a href="https://miktex.org/download">Download</a>

Easy to install <u>but does not ship with Perl, which the `latexmk` package requires.</u>

1. Install MiKTeX using the above link. Then, you have the option to upgrade your installation to a standard TeX system by clicking the `Upgrade` button. Please be aware that this initiates a ~200MB download.
_Alternatively, you can enable the auto-install feature and let MiKTeX install missing packages on-the-fly. You can find this option in the Settings tab._

<h5>On Windows</h5> 

2. Install Perl using **Strawberry Perl**, available [here](http://strawberryperl.com/). Once installed, verify that Perl is available by opening a new command prompt and typing `perl -v`. If installed correctly, you should see the version of Perl that you installed.

3. Verify that both Perl and MiKTeX are in your `PATH` and restart any open command prompts.

4. You should now be able to compile your $LaTeX$ files using MiKTeX.

<h5>On MacOS</h5>

2. Install Perl using **Homebrew**, available [here](https://brew.sh/).

    ```bash
    brew install perl
    ```

    Once installed, verify that Perl is available by opening a new terminal and typing `perl -v`. If installed correctly, you should see the version of Perl that you installed.

3. Add `~/bin` to your `PATH` by including the following line in your `~/.zshrc` file:

    ```bash
    export PATH="/Users/<username>/bin:$PATH"
    ```

    > [!WARNING]  
    > Here, we use the full path instead of `~/bin` or `$HOME/bin` because the `~` and `$HOME` variables do not work in combination with the VS Code `latex-workshop` extension.

4. You should now be able to compile your $LaTeX$ files using MiKTeX.
</td>
</tr>
</table>

<table>
<tr>
<th>
  <img src="https://ctan.org/teaser/pkg/texlive"  height="16" style="margin: 0 6px -2px 0;">
  TexLive
</th>
</tr>
<tr>
<td>
<a href="https://tug.org/texlive/">Website</a>

For more in-depth information, take a look at the [documentation](https://tug.org/texlive/doc.html).

TeX is a really popular distribution. Despite the installation process being quite lengthy, it enables the direct use and compilation of a project using this repository in VSCode, as explained later.

<h5>On Windows</h5>

Follow the [link](https://tug.org/texlive/acquire-netinstall.html), download `install-tl-windows.exe`, and install the distribution just like any other program.

<h5>On MacOS (MacTeX)</h5>

> [!WARNING]  
> The name is different, but it is developed by the same team of programmers. It has **not** been tested whether the operating conditions are identical to those on Windows. Let us know if you are in this situation.

An installation and usage guide is available [here](https://tug.org/mactex/). Do not hesitate to make a PR if you have any information to add.
</td>
</tr>
</table>
<p align="center"><i>Any other LaTeX distribution to suggest?</i></p>

#### Part B: IDE

After installing a LaTeX distribution, you will need an IDE to edit and compile your $LaTeX$ files. Here is a list of tested and working IDEs for this project:

<table>
  <tr>
    <th>
      <img src="https://github.com/Juknum/UTBM-Internship-Report/assets/49886317/dba03968-0b1a-4812-a82d-742ffc8c31a8"  height="16" style="margin: 0 6px -2px 0;">
      Visual Studio Code
    </th>
  </tr>
  <tr>
    <td>
    <a href="https://code.visualstudio.com">Website</a>
      
This template **requires** the use of the [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) extension to compile the $LaTeX$ files directly within VS Code.

While not mandatory, the following extensions are recommended for some Quality of Life improvements:

- 🔸 [LaTeX Utilities](https://marketplace.visualstudio.com/items?itemName=tecosaur.latex-utilities) - Useful extension to extend the capabilities of LaTeX Workshop.
- 🪄 [LaTeX Formatter](https://marketplace.visualstudio.com/items?itemName=nickfode.latex-formatter) - Enhance the code base for a more user-friendly experience.
- 🔦 [LaTeX language support](https://marketplace.visualstudio.com/items?itemName=torn4dom4n.latex-support) - This extension adds syntax highlighting for LaTeX files.
- 📗 [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) - Don't let typos slip through the cracks.

To compile the report, you can use the <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>B</kbd> shortcut or the `LaTeX Workshop: Build LaTeX project` command inside Visual Studio Code.

> [!NOTE]  
> More information on the LaTeX Workshop extension can be found [here](https://github.com/James-Yu/LaTeX-Workshop/wiki/Install).

You can open and use this project by opening the folder in the source control menu (on the left-hand side of the interface) and using this link: `https://github.com/Juknum/UTBM-Internship-Report.git`.
  </tr>
</table>

<p align="center"><i>Any other IDE to suggest?</i></p>

---

<p align="center">
  <i>If you want to contribute to this project, feel free to make a PR 🤍</i>
</p> 
