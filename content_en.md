layout: true

<div class="my-header"></div>

<div class="my-footer">
  <table>
    <tr>
      <td style="text-align:right">Saxon State Library – State and University Library</td>
      <td>20th June 25</td>
      <td style="text-align:right"><a href="https://www.slub-dresden.de/">www.slub-dresden.de</a></td>
    </tr>
    <tr>
      <td style="text-align:right">Research-related services</td>
      <td />
    </tr>
  </table>
</div>

<div class="my-title-footer">
  <table>
    <tr>
      <td style="text-align:left"><b>Kay-Michael Würzner</b></td>
    </tr>
    <tr>
      <td style="text-align:left">Research-related services</td>
    </tr>
    <tr>
      <td style="font-size:8pt"><b>20th June 2025</b></td>
    </tr>
    <tr>
      <td style="font-size:8pt">LaTeX@SLUB</td>
    </tr>
  </table>
</div>

---

class: title-slide
count: false

# LaTeX Modules
## Source Code Listings

---

# Overview

- LaTeX@SLUB
- LaTeX package [`listings`](https://ctan.org/pkg/listings)
- Hands-on in [`ShareLatex`](https://tex.zih.tu-dresden.de/)

---

class: part-slide
count: false

# LaTeX@SLUB

---

# LaTeX@SLUB

.cols[
.fifty[
- LaTeX as part of the library's educational offerings
- **Goals:**
  + Establish LaTeX as a typesetting program
  + Strengthen *computer literacy*
  + Support scientific professionalism
- **Modules:**
  + Zotero & LaTeX, APA-compliant citation, resumes, business letters, source code (tbc.)
]
.fifty[
<img src="img/program_en.svg">
]
]

---

class: part-slide
count: false

# LaTeX Package listings

---

# LaTeX Package listings

- Elements of source code representation as predefined variables, e.g.
  + Language: `language`
  + Indentation depth: `tabsize`
  + Frame: `frame`
- Alternatives, e.g.
  + [verbatim](http://www.weinelt.de/latex/verbatim.html)
  + [fancyvrb](https://ctan.org/pkg/fancyvrb)
  + [minted](https://ctan.org/pkg/minted)
- Comparable concepts, different approaches, i.e.
  + `verbatim`: Basic environment
  + `minted` based on [Pygments](https://pygments.org/)

---

# Alternatives Compared

| Package    | Pros                             | Cons / Prerequisites               |
|------------|----------------------------------|------------------------------------|
| `verbatim` | Built-in, very simple            | No syntax highlighting             |
| `fancyvrb` | Flexible formatting              | Still no highlighting              |
| `minted`   | High-quality coloring via Pygments | Requires Python, shell-escape    |

➡️ **`listings`** great middle-ground option.

---

# Basic Usage 1

```latex
\usepackage{listings}
\lstset{
  language=Python,
  basicstyle=\ttfamily\small,
  keywordstyle=\color{blue},
  commentstyle=\color{gray}\itshape,
  tabsize=2,
  frame=single,
  numbers=left,
  numberstyle=\tiny\color{gray},
  breaklines=true
}
```

---

# Basic Usage 2

```latex
\begin{lstlisting}
def greet(name):
  # Greet the user
  print(f"Hello, {name}!")
\end{lstlisting}
```

✅ Nicely styled, framed, numbered Python code.

---

class: part-slide
count: false

# Demo

---

class: part-slide

# Thank you for your attention!

<center>
<a href="https://wrznr.github.io/latex-modules-listings/#1">wrznr.github.io/latex-modules-listings</a>
</center>
