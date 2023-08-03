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
This repository is a template for internship reports at the UTBM. It is based on the <a href="https://github.com/pinam45/utbm-latex-internship-report-covers">UTBM internship LaTeX version</a> and has been adapted and expanded with multiple functionalities.
</p>

<table>
<tr>
<td>
Table of contents
</td>
</tr>
<tr>
<td>
<ul>
  <li><a href="#i-support">I. Support</a></li>
  <li>
    <a href="#ii-features">II. Usage & Features</a>
    <ul>
      <li><a href="#utbms-covers">UTBM's Covers</a></li>
    </ul>
  </li>
  <li>
    <a href="#iii-usage">III. Usage</a>
    <ul>
      <li><a href="#online">Online</a></li>
      <li>
        <a href="#locally">Locally</a>
        <ul>
          <li><a href="#part-a-latex-distribution">Part A: LaTeX distribution</a></li>
          <li><a href="#part-b-ide">Part B: IDE</a></li>
        </ul>
      </li>
    </ul>
  </li>
</ul>
</td>
</tr>
</table>

## I. Support

This template can be used in several places:

- Online with [Overleaf](https://www.overleaf.com)
- Locally on Windows/MacOS/Linux

---

## II. Features

> **Warning**  
> This template is free to use, but the covers belongs to the [UTBM](https://www.utbm.fr/) and can only be used with their authorization.  

> **Note**  
> UTBM and all UTBM-related trademarks and logos are trademarks or registered trademarks of the [University of Technology of Belfort-Montbéliard](https://www.utbm.fr/) in France, other countries, or both.

### UTBM's Covers

You can find all configurable options of UTBM covers within the below code, but if you feel unhappy you can still edit the covers [with this file here](https://github.com/Juknum/UTBM-Internship-Report/blob/main/libs/utbmcovers.sty).  
<!-- Code block mention (GitHub markdown feature) -->

https://github.com/Juknum/UTBM-Internship-Report/blob/108d23dee1516941a37bd0aa2fcbf109c8e18f6c/main.tex#L32-L55  

You can also modify their colors using those variables:  
<!-- Code block mention (GitHub markdown feature) -->

https://github.com/Juknum/UTBM-Internship-Report/blob/108d23dee1516941a37bd0aa2fcbf109c8e18f6c/libs/utbmcovers.sty#L36-L55  

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

---

## III. Usage

There is multiple way to use this template, you can either use it online or locally:

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
    
1. There is two way to import this template on [Overleaf](https://www.overleaf.com/):  
    - You can either use the "import from GitHub" button, and then paste the link of this repository. (You will need the paid plan to use this method)
    - Or you can download the repository as a zip file and upload it on Overleaf. (You can use this method for free)

2. The last step is to change the compiler from `pdfLaTeX` to `XeLaTeX`, you can do it by clicking on the `Menu` button and then you can find it in the `Settings` category.

    </td>
  </tr>
</table>
<p align="center"><i>Any other online LaTeX editors to suggest?</i><p>

### Locally

Clone this repository using the following command:

```bash
git clone 'https://github.com/Juknum/UTBM-Internship-Report/tree/main'
```

> **Note**  
> You may also want to use this repository as a template, you can do it by clicking on the `Use this template` button or by clicking [here](https://github.com/new?template_name=UTBM-Internship-Report&template_owner=Juknum).

#### Part A: LaTeX distribution

You will need a LaTeX distribution to compile this project locally, here is a list of tested and working distributions for this project:

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

Easy to install <u>but does not ship with Perl which the `latexmk` package requires.</u>

1. Install MiKTeX using the above link. Then you have the option to upgrade your installation to a standard TeX system. Just click the `Upgrade` button. Please be aware that this starts a ~200MB download.  
_Alternatively, you can turn on the auto-install feature and let MiKTeX install missing packages on-the-fly. You can find this option in the Settings tab._

<h5>On Windows</h5> 

2. You can install Perl using **Strawberry Perl**, which is available [here](http://strawberryperl.com/).  
    Once it's installed, you can verify that Perl is available by opening a new command prompt and typing `perl -v`. If it's installed correctly, you should see the version of Perl that you installed.

3. Verify that both Perl and MiKTeX are in your `PATH` and restart any open command prompts.

4. You should now be able to compile your $LaTeX$ files using MiKTeX.

<h5>On MacOS</h5>

2. You can install Perl using **Homebrew**, which is available [here](https://brew.sh/). 

    ```bash
    brew install perl  
    ```

    Once it's installed, you can verify that Perl is available by opening a new terminal and typing `perl -v`. If it's installed correctly, you should see the version of Perl that you installed.

3. Add `~/bin` to your `PATH` by adding the following line to your `~/.zshrc` file: 

    ```bash
    export PATH="/Users/<username>/bin:$PATH"
    ```

    > **Warning**  
    > Here we use the full path instead of using `~/bin` or `$HOME/bin` because the `~` and `$HOME` variables does not works if used in combination with the VS Code `latex-workshop` extension.

4. You should now be able to compile your $LaTeX$ files using MiKTeX.
</td>
</tr>
</table>

<p align="center"><i>Any other LaTeX distribution to suggest?</i></p>

#### Part B: IDE

After installing a LaTeX distribution, you will need an IDE to edit and compile your $LaTeX$ files, here is a list of tested and working IDEs for this project:

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

This template **require** the use of the [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) extension to compile the $LaTeX$ files directly within VS Code.

While they are not required to use the template, the following extensions are recommended for some Quality of Life improvements:

- 🔸 [LaTeX Utilities](https://marketplace.visualstudio.com/items?itemName=tecosaur.latex-utilities) - Useful extension to extends capabilities of LaTeX Workshop.
- 🪄 [LaTeX Formatter](https://marketplace.visualstudio.com/items?itemName=nickfode.latex-formatter) - Appreciate a more user friendly code base.
- 🔦 [LaTeX language support](https://marketplace.visualstudio.com/items?itemName=torn4dom4n.latex-support) - This extension adds syntax highlighting for LaTeX files.
- 📗 [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) - Don't let typos slip through the cracks.

To compile the report, you can use the <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>B</kbd> shortcut or the `LaTeX Workshop: Build LaTeX project` command inside Visual Studio Code.

> **Note**  
> More information on the LaTex Workshop extension can be found [here](https://github.com/James-Yu/LaTeX-Workshop/wiki/Install).
    </td>
  </tr>

</table>

<p align="center"><i>Any other IDE to suggest?</i></p>

---

<p align="center">
  <i>If you want to contribute to this project, feel free to make a PR 🤍</i>
</p> 
