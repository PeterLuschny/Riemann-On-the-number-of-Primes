
It is very easy to convert the html file into a LaTeX file:

(1) Save a copy of the Html file and change the file-suffix to ".tex".
    Delete all lines before the first line of Riemann's text starting
    "The best way to express ..." and after the last line of the text.

(2) Use an editor to

    delete  all <p>
    delete  all </p>
    delete  all <p style="color:maroon">
    replace all \gt   by >
    replace all &amp; by &
    replace all ß     by {\ss}

(3) Insert the next lines at the beginning of the file:

    \documentclass[a4paper,12pt]{article}
    \usepackage[a4paper, left=5cm, textwidth=10cm]{geometry}
    \RequirePackage{amsmath}
    \RequirePackage[pdftex]{hyperref}
    \title{On the Number of Primes less than a given Magnitude}
    \author{Bernhard Riemann} \date{\vspace{-4ex}}
    \begin{document}
    \maketitle

    and insert the line
        \end{document}
    at the end of the file.

(4) Save the file and compile. This should result in a pdf-file
    assuming you have a working TeX environment.
