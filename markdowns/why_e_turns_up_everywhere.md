# Why $e$ Turns Up Everywhere

As the previous section showed, $e$ is the one base whose exponential function reproduces itself under differentiation. That property is elegant on its own, but its real importance lies in what it means outside of pure mathematics: it is exactly the condition satisfied by any process whose rate of change depends on how much of it already exists.

A larger population produces more births. A larger investment earns more interest. A larger quantity of radioactive material produces more decay events. In each case, growth or decay feeds on its own current size.

Calculus describes these situations using differential equations, and the solutions repeatedly involve the exponential function $e^x$.

As a result, the same number that appeared in logarithms, compound interest, and infinite series turns out to reappear throughout science — and, as the three examples below show, throughout nature itself.

## Population Growth

Imagine a colony of bacteria in a petri dish, with unlimited food and no predators in sight. Every bacterium divides in two after a fixed amount of time, so the more bacteria there are, the faster new bacteria appear.

This is the defining feature of exponential growth: the rate of increase is proportional to the current size. Mathematically, that idea is written as a simple differential equation:

$$
\frac{dP}{dt} = kP
$$

Here $P$ is the population and $k$ is the growth rate. Solving this equation gives:

$$
P(t) = P_0 \, e^{kt}
$$

where $P_0$ is the starting population. Notice that $e$ appears not because anyone inserted it by hand, but because it is the only base for which this growth pattern works out cleanly.

Of course, real populations rarely grow forever — food runs out, predators arrive, space becomes limited. But in the short term, from bacteria in a dish to rabbits in a field to cells in a growing tumor, this same exponential curve shows up again and again. Wherever "more now means more later," $e$ is quietly running the numbers.


## The 37% Rule

*$e$ and the search for happiness*

There is also a playful little surprise involving $e$.

In a famous problem called the **optimal stopping problem**, $e$ appears in a very unexpected way.

The basic question is this:

Suppose you must choose the best candidate from a sequence of candidates. You interview them one at a time. Once you reject someone, you cannot go back. So what is the best strategy?

A classic mathematical answer says: first, reject approximately

$$
\frac{1}{e}
$$

of the candidates. Since

$$
\frac{1}{e} \approx 0.3679
$$

this means rejecting about $37\%$ of the candidates before making a serious choice — then settling for the very next one who beats everyone you've seen so far.

When searching for a partner, the best strategy, apparently, is to reject the first $1/e$ possibilities — that is, the first 37% — and then commit to the first new candidate who is better than all the ones you turned down.

I say "apparently," because I haven't actually tried it.

## Logarithmic Spirals

There is a curve that nature seems to love, and $e$ is hiding right inside its formula.

It's called the **logarithmic spiral**, and its equation looks like this:

$$
r = a \cdot e^{b\theta}
$$

Here, $r$ is the distance from the center, $\theta$ is the angle of rotation, and $a$ and $b$ are constants that control the size and tightness of the spiral.

What makes this curve special is that it grows *exponentially* as it turns — every time it rotates by a fixed angle, it expands by the same **proportion**, not the same amount.

This self-similar growth pattern shows up again and again in the natural world:

- The chambers of a **nautilus shell**, each one a scaled-up copy of the last
- The swirling arms of a **hurricane**, viewed from above
- The sweeping arms of a **spiral galaxy**
- Even the curl of a **ram's horn** or a **fern frond** unfurling



**Caption:** *A nautilus shell cross-section, showing the logarithmic spiral $r = a \cdot e^{b\theta}$ traced by its chambers.*

Mathematicians sometimes call it the *"spira mirabilis"* — the miraculous spiral — a name the astronomer Jacob Bernoulli gave it because he was so charmed by its self-repeating growth that he asked for it to be engraved on his tombstone.
