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

    \documentclass[english,a4paper,12pt]{article}
    \usepackage[utf8]{inputenc}
    \usepackage[T1]{fontenc}
    \usepackage{babel}
    \usepackage[a4paper, left=5.5cm, textwidth=10cm]{geometry}
    \RequirePackage{amsmath}
    \RequirePackage[pdftex]{hyperref}
    \def\Li{\operatorname{Li}}
    \title{On the Number of Primes less than a given Magnitude}
    \author{Bernhard Riemann} \date{\vspace{-4ex}}
    \begin{document}
    \maketitle

    and insert the line
        \end{document}
    at the end of the file.

    For the French version replace the first line by
        \documentclass[french,a4paper,12pt]{article}
    and the title line by
        \title{Sur le nombre de nombres premiers inférieurs à une taille donnée}

(4) Save the file and compile. This should result in a pdf-file
    assuming you have a working TeX environment.

Here you can see a preview of the [Englich version](http://luschny.de/math/zeta/OnTheNumberOfPrimesLessThanAGivenMagnitude.pdf)
and of the [French version](http://luschny.de/math/zeta/SurLeNombresPremiers.pdf).
