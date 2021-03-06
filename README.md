This project has a twofold objective:

(A) To provide a translation of classical work "�ber die Anzahl der
    Primzahlen unter einer gegebenen Gr��e" by Bernhard Riemann to English.

(B) To give the text a format which can be used for comfortable reading
    on a mobile device.

The decisive factor for (A) was that apparently no translation exists
that has a free license (the Riemann's text itself is free).

For (B) we have as target reader in mind a student who on the way to the
university in the subway is reading the text on his mobile phone or tablet.

To this end, we set the following goals:

(0) The translation is released worldwide into the public domain.
    (CC zero license).

(1) The translation aims to be in today's colloquial English and does
    not attempt to reconstruct the nested sentences of the academic
    language of the 19th century Riemann uses. Readability is sought,
    not a philological transcription.

(2) No comments or remarks. Such can be found in their thousands on the
    Internet. The presentation should concentrate on the pure text.

(3) The known minor errors are *silently* corrected. This means in
    particular:

    (a) the forgotten sum sign on page 4 of the Monthly Report of the
        Academy is inserted, as it is in the collected works.

    (b) Typos like (x)psi -> psi(x).

    (c) Also the well-known 'lapsus calami' is corrected,
        so log xi(0) is set to -log 2.

(4) Use of modern function names. This means three things:

    (a) The factorial function, which Riemann denotes by ProductPi is
        replaced by Legendre's Gamma function.
        [ProductPi(x) -> Gamma(x+1)]

    (b) pi(x) denotes the number of primes less than or equal to x as
        it is common nowadays. Riemann calls this function F(x).
        [F(x) -> pi(x)]

    (c) Pi(x) is defined as Sum_{n>=1} pi((1/n) x^(1/n)). Riemann calls
        this function f(x).
        [f(x) -> Pi(x)]

   For example this notation is used by Ricardo P�rez-Marco in "Notes
   on the Riemann Hypothesis".

(5) The text format is Html and LaTex/MathJax. This is supposed to
    be as slender as possible and to be easy to read on small devices
    like smartphones and tablets.

(6) If you discover errors or have suggestions for improvement
    please send a pull request.

Here you can see a [preview](http://luschny.de/math/zeta/OnTheNumberOfPrimesLessThanAGivenMagnitudeMerriweather.html).
A French version using the translation of [Laugel](http://luschny.de/math/zeta/SurLeNombresPremiersOldStandard.html).
