# Latex Template Documentation

1. [Setup LaTeX in Atom](#setup-latex-in-atom)

## Setup LaTeX in Atom

### Required settings:

1. Download and install [Perl](https://www.perl.org/get.html)
2. Download and install [MiKTeX](https://miktex.org/download)
3. Download and install [Atom](https://atom.io/)
4. Open Atom
5. Press 'ctrl + ,' to open settings
6. Open the install tab
7. Install the following packages by writing the names in the search bar

    required:

    - latex - (required, ability to compile latex)

    ---

    optional (but highly recommended):

    - language-latex (syntax highlighting, makes the tex file much easier to read)
    - latex-autocomplete (helps you to create figures, items, etc.)
    - autocomplete-latex (helps you to create figures, items, etc.)
    - pdf-view - (required, shows the compiled latex file in the editor)

### Optional settings:

#### 'latex' package settings:

- Ouput Directory: saves the meta files in the defined directory, this helps to keep your root directory clean
- Move Result to Source Directory: saves the pdf file in the same folder as the producing tex document
- Build on Save: starts a build when the file is safed ('ctrl + s' or by clicking 'File>Save..')
- Open Result after Successful Build: opens the pdf in the 'pdf-view' after the build finished

**To edit the settings:**

1. Open packages tab in the settings window
2. Search for the package latex and open the package settings

#### 'spell-check' package settings:

- Grammars: the file types that will be spell checked
- Use Locales: if locals should be used for the spell check
- Locales: what locals should be used for the spell check (example: en-US, de-DE)

**To edit the settings:**

1. Open packages tab in the settings window
2. Search for the package 'spell-check' and open the package settings
3. Add 'text.tex.latex' and the end of the field 'Grammars'
4. Enable 'Use Locals'
5. Add desired language to 'Locales' (for german add: 'de-DE')
> To add support for more languages in 'Locales', check [here](https://atom.io/packages/spell-check) in the 'Changing the dictionary' section

## LaTeX Introduction

### Hierarchy
**Input:**

```latex
\chapter{chapter}
\section{section}
\subsection{sub section}
```
**Output:**

![hierarchy-image](https://user-images.githubusercontent.com/47224024/98449617-37517280-2135-11eb-86d5-0534ca5cbf4b.png)

### Figure
**Input:**
```latex
\begin{figure}[H]                             %H to display it exactly where its in the code
\center                                       %centers image
\includegraphics[scale = 0.3]{Logo}           %image in 'pictures' directory, scaled down to 30%
\caption{caption}                             %will be the caption of the image
\label{fig:Logo}                              %used for reference in text
\end{figure}
```
**Output:**

![figure-image](https://user-images.githubusercontent.com/47224024/98449863-dbd4b400-2137-11eb-8dfb-97e32a30c0d1.png)
