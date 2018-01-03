# Arbeidskrav 2 (individuelt)

Betrakt en pendel bestående av en punktmasse $m$ som henger i en stiv,
masseløs stav med lengde $L$ i et gravitasjonsfelt $g$. La $\theta(t)$
betegne vinkelen som pendelen utgjør med loddlinjen som funksjon av
tiden. Pendelen slippes i en vinkel $\theta(0) = \theta_0$, i ro,
$\theta'(0) = 0$.

# Bevegelsesligningen

Gjenoppfrisk mekanikkunnskapene og vis at bevegelsesligningen for
pendelen er

$$
\frac{d^2\theta}{dt^2} = -\frac{g}{L}\sin\theta,
$$

en ikkelineær ordinær differensialligning av andre orden.

# Tilnærmet ligning

For små vinkler, $\theta\ll1$, er $\sin\theta\approx\theta$, og
bevegelsesligningen kan tilnærmes som 

$$
\frac{d^2\theta}{dt^2} = -\frac{g}{L}\theta.
$$

Løs denne lineære ordinære differensialligningen analytisk for
initialverdiene gitt over, og vis at pendelens periode er $T =
2\pi\sqrt{L/g}$.

# Numerisk løsning av den tilnærmede ligningen

Introduser $\phi = d\theta/dt$ og skriv den tilnærmede ligningen som
et system av to lineære førsteordens ligninger. Utled numeriske
skjemaer for å løse denne vha. eksplisitt Euler, implisitt Euler, Heun
og Crank--Nicholson. Implementer numerisk (bruk $g = L = 1$ for
enkelhets skyld), løs for forskjellige tidsskritt og sammenlign
nøyaktigheten av perioden med den eksakte løsningen. Plot $\theta(t)$
for noen få perioder for de ulike skjemaene.

# Numerisk løsning av den eksakte ligningen

Introduser $\phi = d\theta/dt$ og skriv den eksakte ligningen som et
system av to ikkelineære førsteordens ligninger. Utled numeriske
skjemaer for eksplisitt Euler og Heun (hvorfor ikke implisitt og
Crank--Nicholson?). Implementer numerisk (bruk $g = L = 1$ for
enkelhets skyld), løs for forskjellige tidsskritt og forskjellige
verdier av $\theta_0$, og sammelign nøyaktigheten med den eksakte løsningen,

$$
T = 2\pi\sqrt{g/L}
    \left(1 + \frac{1}{16}\theta_0^2 +
    \frac{11}{3072}\theta_0^4 + \cdots\right).
$$

Plot $\theta(t)$ for noen få perioder for de forskjellige skjemaene og
forskjellige verdier av $\theta_0$.


# Ekstra: animasjon

Lag en fin animasjon av den svingende pendelen!
