# Introduction

## A Number Nobody Was Looking For

Let us begin with a question:

**What do astronomy, banking, calculus, radioactive decay, and population growth have in common?**

Most people would probably answer:

> “Common? They all make me want to take a nap?”

Fair enough. That is not entirely wrong. But a mathematician would give something else:

> They all eventually lead to the same number:
>
> $$e \approx 2.71828$$

---
$e$ is a weird number.

Unlike $\pi$, which arrives with circles and geometry, $e$ is much harder to recognize. There is no obvious shape associated with it, no famous theorem named after it, and no simple visual interpretation that makes it instantly memorable.

In fact, nobody was deliberately searching for it. 

$e$ emerged gradually from a collection of seemingly unrelated problems—astronomical calculations, logarithms, compound interest, and eventually calculus itself.
Only later did mathematicians realize that all of these paths were leading to the same destination.

That realization is what makes the history of $e$ feel like a mathematical detective story: **The clues appeared first. The number came later.**

---

# Chapter 1 Astronomers Were Drowning in Arithmetic

Long before anyone recognized the number $e$, astronomers were struggling with a much more immediate problem: calculation.

Modern astronomy sounds exciting—stars, planets, galaxies, and the mysteries of the universe. But for astronomers in the sixteenth and seventeenth centuries, much of the work involved pages upon pages of arithmetic. Predicting planetary motion, constructing calendars, and navigating across oceans all required enormous amounts of multiplication and division.

[a picture of struggle astronomy]

Without calculators or computers, these computations were slow, tedious, and prone to error. A small mistake could ruin an astronomical prediction or send a ship off course. As a result, mathematicians began searching for faster and more reliable ways to calculate.

This led mathematicians to a practical question:

> **Could multiplication somehow be turned into something easier?**

The idea sounds simple, but its consequences were revolutionary. 

# Chapter 2 John Napier's Shortcut

## Turning Multiplication into Addition

> Seeing there is nothing that is so troublesome to mathematical practice, nor that doth more molest and hinder calculators, than the multiplications, divisions, square and cubical extractions of great numbers. . . . I began therefore to consider in my mind by what certain and ready art I might remove those hindrances *-John Napier (1614)*

The Scottish mathematician **John Napier** took up this challenge. Born near Edinburgh in 1550, Napier was not a professional scientist in the modern sense but a scholar and landowner with a deep interest in mathematics. As astronomical observations became increasingly precise and scientific calculations grew ever more demanding, he became fascinated by the enormous amount of arithmetic required to support them.

[picture of napier]

Determined to reduce this burden, Napier devoted nearly twenty years to develop a new computational method. His efforts culminated in the publication of logarithms in 1614—an invention that transformed scientific calculation for centuries.

Today, logarithms are usually introduced through exponents. Although Napier's original construction was quite different, it embodied the same fundamental idea: **turning multiplication into addition.**

For modern readers, this idea is most easily understood through exponents. Consider the familiar law

$$
10^a \times 10^b = 10^{a+b}.
$$

The equation shows that multiplication can be encoded as addition when numbers are represented through exponents. Logarithms capture this relationship through the identity

$$
\log(ab)=\log(a)+\log(b).
$$

This formula may appear routine for modern readers. In the seventeenth century, however, it offered a completely new way to think about calculation. Multiplications that once required substantial effort could now be reduced to additions, dramatically decreasing both the time required and the likelihood of error. In principle, astronomers no longer needed to multiply enormous numbers directly; they only needed to add their logarithms.

[napier's original way of doing this, maybe use a callout with header]

## Briggs and the Decimal Revolution

Napier's invention attracted immediate attention across Europe. Among the mathematicians who studied it most closely was the English mathematician **Henry Briggs**.

Briggs realized that logarithms would be even more practical if they were built around powers of ten. Because everyday arithmetic already used the decimal system, base-10 logarithms were easier to compute and easier to use. Working closely with Napier, Briggs developed extensive decimal logarithm tables that quickly became the standard throughout Europe.

The process of using a logarithm table was straightforward:  
- Look up the logarithms of the specific numbers being multiplied.
-  Add these logarithmic values together.  
- Perform a reverse lookup in the table to translate the sum back into the final result.

[include a log table]

For scientists of the seventeenth century, these tables were revolutionary. Astronomers, navigators, surveyors, and engineers relied on them to perform calculations that would otherwise have required enormous effort.

Yet the success of base 10 raised a subtle question. If logarithms could be built from powers of ten, could they also be built from other bases? And if so, was there a base that was mathematically more natural than the others?

At the time, nobody knew the answer.

---

# Chapter 3 Bernoulli's Question

For decades, Napier's clue remained hidden. His computation scheme had transformed calculation, but no one recognized that they contained a deeper mathematical constant.

Then the trail resurfaced in an unexpected place. Not in astronomy, navigation, or geometry, but in a question that concerned merchants and bankers alike: how does money grow when interest is compounded again and again?

## Can A Bank Account Grow Forever?

By the late seventeenth century, compound interest had become an important practical problem for merchants, lenders, and bankers. As financial transactions grew more sophisticated, mathematicians became increasingly interested in understanding how investments behaved over long periods of time.

Among them was **Jacob Bernoulli**. He was interested in a question about compound interest: If money earns interest not just once per year, but repeatedly throughout the year, how much can an investment ultimately grow?

To explore the question, he began with a simple example.

Suppose you have one unit of currency invested, earning a highly generous 100% annual interest rate. Instead of receiving the entire 100% at the end of the year, imagine the interest is split equally among $n$ compounding periods. Each period then contributes a rate of $\frac{1}{n}$, so the account is multiplied by $1+\frac{1}{n}$ each time. After $n$ such periods, the final amount becomes

$$\left(1+\frac{1}{n}\right)^n$$

As Bernoulli pushed the compounding frequency higher, a clear pattern emerged:
| Compounding Frequency | Formula | Final Amount |
|---|---|---|
| Annually ($n = 1$) | $(1 + 1/1)^1$ | 2.00000 |
| Quarterly ($n = 4$) | $(1 + 1/4)^4$ | 2.44141 |
| Monthly ($n = 12$) | $(1 + 1/12)^{12}$ | 2.61303 |
| Weekly ($n = 52$) | $(1 + 1/52)^{52}$ | 2.69260 |
| Daily ($n = 365$) | $(1 + 1/365)^{365}$ | 2.71457 |
| Hourly ($n = 8760$) | $(1 + 1/8760)^{8760}$ | 2.71813 |


## A Pure Number Appears

Bernoulli noticed a profound paradox. Increasing the compounding frequency certainly increases the final amount. However, each increase contributes less than the one before it. The gains keep accumulating, yet they do so at a diminishing rate.

This raises a natural question:

> Is there an ultimate limit to how much extra growth can be squeezed out of compounding?

As the number of compounding periods grows without bound, the expression
$
\left(1+\frac{1}{n}\right)^n
$
approaches a specific number:

$$
2.71828\ldots
$$

Bernoulli had uncovered something unexpected. A problem about compound interest seemed to be approaching a specific numerical limit, one that did not depend on any particular bank, currency, or investment. The result looked less like a fact about finance and more like a property of mathematics itself.

Yet its significance remained unclear. Bernoulli had found the number, but not its place in the larger mathematical landscape. That connection would only become visible later.

---

# Chapter 4 Euler Connects the Dots

## A Different Base

By the eighteenth century, logarithms had become indispensable scientific tools. Briggs's base-10 tables were used throughout Europe, and for practical computation there seemed to be little reason to prefer any other system.

Yet mathematicians knew that logarithms could be constructed using many different bases. For example,
$
\log_{10}(100)=2
$
simply means that
$
10^2=100.
$

But there is nothing inherently special about the number 10. It is the base we use because our number system is decimal. Other bases work just as well:

$$
\log_2(2^3)=3,
\qquad
\log_3(3^4)=4.
$$

Napier and Briggs had built logarithms as a computational tool — a table you looked things up in. Back then, nobody was asking whether one base was more "correct" than another. That question only became possible once mathematicians started treating logarithms not as tables, but as *functions*.

## Euler's Bigger Project

That shift had already begun before Euler arrived on the scene. In 1697, **Johann Bernoulli** — Jacob's younger brother — started developing what he called a calculus of exponential functions, studying expressions like $a^x$ using the new tools of differentiation and integration. Logarithms, in this view, were simply the inverse of exponentials: if $a^y=x$, then $y$ is the logarithm of $x$ to base $a$.

Then, **Leonhard Euler** picked up this thread in the 1720s and 1730s as part of a much larger ambition: to put the whole of algebra and calculus — powers, logarithms, exponentials, trigonometry — on one unified, systematic footing. This project would eventually culminate in his 1748 textbook, the *Introductio in Analysin Infinitorum*.

It was while working through exponential functions in this broader context, not while chasing a single isolated riddle, that Euler ran into the question left dangling since Napier's research:

> If a logarithm is really just the inverse of an exponential function, is there a base whose exponential function behaves most simply under calculus?

## The Constant Reappears

To compare bases, Euler looked at how $a^x$ changes. Differentiating it produces the exponential function back again, multiplied by a leftover constant that depends on the base:

$$
\frac{d}{dx}a^x=\lim_{h\to 0}\frac{a^h-1}{h}\cdot a^x.
$$

For most bases this limit is an unremarkable, forgettable number. Euler wanted to know: is there a number $a$ for which the limit simply equals 1 — a base whose exponential function is its own derivative?

Working out which number satisfies this condition led straight back to an old acquaintance. The value turned out to be exactly the limit Jacob Bernoulli had run into decades earlier while compounding interest:

$$
e=\lim_{h\to 0}\left(1+h\right)^{\frac1h}=\lim_{n\to\infty}\left(1+\frac1n\right)^n\approx 2.71828\ldots
$$

Bernoulli had been asking a question about money. Euler was asking a question about calculus. Both roads ended at the same number.

[fun fact about the naming of e]

## One Number, Two Faces

Euler didn't stop at the limit. A limit is easy to state but slow to compute — plugging in a huge $n$ only ever gives an approximation. So Euler also worked out a second way to express the same constant, as an infinite sum:

$$
e=1+\frac1{1!}+\frac1{2!}+\frac1{3!}+\cdots
$$

This series converges quickly — a handful of terms already nails down several decimal places — which made it far more useful for actual calculation than the original limit. More importantly, Euler showed that the limit and the series were two descriptions of the very same number. Bernoulli's compound-interest problem and this new infinite sum were not just similar; they were identical.

## Logarithms and Exponentials, Reunited

By the time Euler came to the problem, the area under $y=\frac1x$, which is
 $$\int_1^x \frac1t dt$$
 
 was already known to behave like a logarithm. That function had a name by then: **the natural logarithm**, while back then, the base for this 'natural logarithm' was still unknown.
 
[a demo for how this area act like log]

Euler's key step was to recognize that the constant appearing when you differentiate $a^x$ is the same function, and the constant $e$ was exactly the base for this secret logarithm:
develop
$$
lim_{h\to 0}\frac{a^h-1}{h}=\int_1^a \frac1t dt=\ln a.
$$

Although the symbol $ln$ was introduced later, it represents the same logarithmic function that Euler identified. Once $e$ is chosen so that $\ln e=1$, the special case becomes

$$
\ln e = 1,
\qquad
\frac{d}{dx}e^x=e^x,
\qquad
\frac{d}{dx}\ln x=\frac1x.
$$

No other base gives this clean a pair of relationships — every other exponential drags along an extra factor of $\ln a$. Base 10 was convenient because we have ten fingers; base $e$ was, in Euler's hands, the base calculus itself pointed to.

This is the shape of the story as it's usually retold today, with the pieces arranged for clarity. Euler's actual notebooks show the ideas arriving more gradually, tangled up with his broader work on infinite series, complex numbers, and trigonometry. But the destination was the same: Napier's computational shortcut, Bernoulli's compound-interest limit, and Euler's calculus of exponentials all turned out to be describing one and the same number.

For the first time, the pieces that had accumulated over more than a century finally fit together.

[include a timeline]

# Chapter 5 Why $e$ Turns Up Everywhere


As Chapter 4 showed, $e$ is the one base whose exponential function reproduces itself under differentiation. That property is elegant on its own, but its real importance lies in what it means outside of pure mathematics: it is exactly the condition satisfied by any process whose rate of change depends on how much of it already exists.

A larger population produces more births. A larger investment earns more interest. A larger quantity of radioactive material produces more decay events. In each case, growth or decay feeds on its own current size.

Calculus describes these situations using differential equations, and the solutions repeatedly involve the exponential function $e^x$.

As a result, the same number that appeared in logarithms, compound interest, and infinite series turns out to reappear throughout science.

### Population Growth

A simple population model can be written as

$$
P(t)=P_0e^{rt},
$$

where $P_0$ is the initial population and $r$ is the growth rate.

### Radioactive Decay

Radioactive substances follow a similar law:

$$
N(t)=N_0e^{-\lambda t},
$$

where $\lambda$ measures how quickly the material decays.

### Electricity

In electrical circuits, the voltage across a discharging capacitor often behaves like

$$
V(t)=V_0e^{-t/RC}.
$$

The details differ, but the mathematical structure is the same. Whenever the rate of change depends on the amount currently present, $e$ tends to appear.

fun fact of different fields use different base

# Conclusion

## The Number That Never Left

The story of $e$ did not begin with someone searching for a special constant.

Napier wanted faster calculations. Bernoulli investigated compound interest. Euler connected seemingly unrelated discoveries into a single mathematical framework. 

At every turn, mathematicians pursued different problems, each following their own line of inquiry. Yet the same constant kept appearing, surfacing again and again in their results.

The journey of $e$ spans astronomy, finance, logarithms, infinite series, and calculus. What makes this remarkable is not merely that the number appears in many places, but that these appearances were discovered independently before anyone realized they were connected.

That is what makes the story of $e$ unusual. It was not invented, designed, or chosen. It revealed itself gradually, appearing wherever the mathematics of growth, change, and accumulation was pushed far enough.
The number nobody was looking for had been there all along.
