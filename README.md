# The Rudin Project
The purpose of this repository is to completely solve all exercises in Walter Rudin's Principles of Mathematical Analysis.

## Usage
If you're just interested in reading the solutions, simply clone this repository and compile `rudin.tex` using your preferred LaTeX distribution

If you would like to contribute, please get in contact with me and I can make you a contributor.

## Guidelines for contributing
This project consists of a master file `rudin.tex`, which `\include`s the eleven `chapter1.tex`,..., `chapter11.tex` chapter files. Global style definitions, packages and macros should appear in `rudin.tex`, while actual solutions should be included in the chapter files.

To format the exercises and their solutions, we are using the exam document class. Features beyond what is described below should not be needed, but you can find the documentation [here](https://www.ctan.org/tex-archive/macros/latex/contrib/exam?lang=en) if you are interested.

The structure of a chapter file will be as follows

'''
\section{Chapter Title}

\begin{questions}
\question Statement of Exercise 1
\begin{solution}
  Solution to Exercise 1
\end{solution}

...

\question Statement of final exercise
\begin{solution}
  Solution to final exercise
\end{solution}
\end{questions}
'''

Please note that indentation is using two spaces -- please change the settings in your editor appropriately (i.e. don't use TABs).

### Macros
Please make use of the following macros. Any other common commands may be turned into macros where appropriate. These can also be seen in the file `rudin.tex`

 * Sets of numbers: `\C`, `\N`, `\Q`, `\R`, `\Z` produce blackbold C, N, Q, R, Z, denoting the sets of complex, natural, rational, real numbers and integers respectively.
 * Absolute Value: `\abs{expr}` produces `|expr|`. For a version which resizes the brackets automatically use `\abs*{expr}`
 * Norm: `\norm{expr}` produces `||expr||`. For a version which resizes the brackets automatically use `\norm*{expr}`
 * Vectors: `\vec{v}` produces **v**
 * Complex Conjugation: `\conj{z}` produces the complex conjugate of `z`
