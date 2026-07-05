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

a picture of struggle astronomy

Without calculators or computers, these computations were slow, tedious, and prone to error. A small mistake could ruin an astronomical prediction or send a ship off course. As a result, mathematicians began searching for faster and more reliable ways to calculate.

This led mathematicians to a practical question:

> **Could multiplication somehow be turned into something easier?**

The idea sounds simple, but its consequences were revolutionary. 

# Chapter 2 John Napier's Shortcut

## Turning Multiplication into Addition

> Seeing there is nothing that is so troublesome to mathematical practice, nor that doth more molest and hinder calculators, than the multiplications, divisions, square and cubical extractions of great numbers. . . . I began therefore to consider in my mind by what certain and ready art I might remove those hindrances *-John Napier (1614)*

The Scottish mathematician **John Napier** took up this challenge. Born near Edinburgh in 1550, Napier was not a professional scientist in the modern sense but a scholar and landowner with a deep interest in mathematics. As astronomical observations became increasingly precise and scientific calculations grew ever more demanding, he became fascinated by the enormous amount of arithmetic required to support them.

Determined to reduce this burden, Napier devoted nearly twenty years to develope a new computational method. His efforts culminated in the publication of logarithms in 1614—an invention that transformed scientific calculation for centuries.

Today, logarithms are usually introduced through exponents. Although Napier's original construction was quite different, it embodied the same fundamental idea: **turning multiplication into addition.**

For modern readers, this idea is most easily understood through exponents. Consider the familiar law

$$
10^a \times 10^b = 10^{a+b}.
$$

The equation shows that multiplication can be encoded as addition when numbers are represented through exponents. Logarithms capture this relationship through the identity

$$
\log(ab)=\log(a)+\log(b).
$$

For modern readers, this formula may appear routine. In the seventeenth century, however, it offered a completely new way to think about calculation. Multiplications that once required substantial effort could now be reduced to additions, dramatically decreasing both the time required and the likelihood of error. In principle, astronomers no longer needed to multiply enormous numbers directly; they only needed to add their logarithms.

napier's original way of doing this

## Briggs and the Decimal Revolution

Napier's invention attracted immediate attention across Europe. Among the mathematicians who studied it most closely was the English mathematician **Henry Briggs**.

Briggs realized that logarithms would be even more practical if they were built around powers of ten. Because everyday arithmetic already used the decimal system, base-10 logarithms were easier to compute and easier to use. Working closely with Napier, Briggs developed extensive decimal logarithm tables that quickly became the standard throughout Europe.

The process of using a logarithm table was straightforward:  
- Look up the logarithms of the specific numbers being multiplied.
-  Add these logarithmic values together.  
- Perform a reverse lookup in the table to translate the sum back into the final result.

include a log table

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

Suppose you have a RM1 initial investment that earns a highly generous 100% annual interest rate. Instead of receiving the entire 100% at the end of the year, imagine the interest is split equally among $n$ compounding periods. Each period then contributes a rate of $\frac{1}{n}$, so the account is multiplied by $1+\frac{1}{n}$ each time. After $n$ such periods, the final amount becomes

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

Bernoulli noticed a profound paradox. Increasing the compounding frequency certainly increases the final amount. However, look closely at the table: the jump from quarterly to monthly is large, but the jump from daily to hourly is tiny. Each subsequent increase becomes progressively smaller than the previous one. By compounding the interest an infinite number of times, the expression $(1+\frac{1}{n})^{n}$ intuitively converges to a pure, finite limit.  That absolute limit is 

$$2.71828...$$

Bernoulli had uncovered something unexpected. A problem about compound interest seemed to be approaching a specific numerical limit, one that did not depend on any particular bank, currency, or investment. The result looked less like a fact about finance and more like a property of mathematics itself.

Yet its significance remained unclear. Bernoulli had found the number, but not its place in the larger mathematical landscape. That connection would only become visible later.

---

# Chapter 4 Euler Connects the Dots

## A Different Base

By the eighteenth century, logarithms had become indispensable scientific tools. Briggs's base-10 tables were used throughout Europe, and for practical computation there seemed to be little reason to prefer any other system.

Yet mathematicians gradually realized that logarithms could be constructed using many different bases. This raised a natural question:

> Was base 10 merely convenient, or was it mathematically special?

Leonhard Euler became deeply interested in this question while studying logarithms, exponential functions, and the emerging ideas of calculus.

As he explored these subjects, he found that one particular base possessed remarkably elegant mathematical properties. The number associated with that base was approximately

$$
2.71828...
$$

The same mysterious value that Bernoulli had encountered in his compound-interest problem!

## A Natural Logarithm

Euler discovered that this number was closely tied to a special exponential function, now written as
$
e^x.
$

fun fact: naming e

Unlike other exponential functions, it behaved with unusual simplicity and elegance. Formulas involving this function were often shorter, cleaner, and easier to manipulate than their counterparts built from other bases. 

The more Euler investigated it, the less it looked like a numerical coincidence and the more it seemed to be a fundamental feature of mathematics itself.

Moreover, he found that the mysterious number could also be represented by the infinite series

$$
e
=
1+1+\frac1{2!}+\frac1{3!}+\frac1{4!}+\cdots
$$

This expression looks completely different from Bernoulli's compound-interest limit

$$
\left(1+\frac1n\right)^n.
$$

One emerges from an infinite sum, while the other arises from repeated compounding. Yet both converge to exactly the same value.

Euler then realized that the same constant governed both a special exponential function and a special logarithm.

What seemed to be unrelated discoveries were gradually revealed to be different expressions of the same mathematical object.

## Why This Base?

At this point, however, a natural question remained.

Why this base?

After all, exponential functions can be built from any positive number. Why should the base e deserve special attention?

The answer came from calculus.

For a general exponential function,

$$
\frac{d}{dx}a^x
=
a^x\ln a.
$$

Most exponential functions return with an extra factor attached.

But when the base is exactly e,

$$
\frac{d}{dx}e^x=e^x.
$$

The function reproduces itself perfectly under differentiation.

Among all exponential functions, it is the only one with this property.

---

For the first time, logarithms, exponential growth, infinite series, and Bernoulli's limit could all be understood within a single mathematical framework.

The pieces that had accumulated over more than a century were finally connected. What began as a computational shortcut for astronomers had evolved into a fundamental structure underlying calculus itself.

**Napier (1614) → Bernoulli (1683) → Euler (1737)**

# Chapter 5

## Why Calculus Loves $e$

By the time Euler connected the dots, $e$ had already appeared in logarithms, compound interest, and infinite series. But none of these discoveries explain why $e$ eventually became known as the **natural base**.

The answer comes from calculus.

Calculus is the mathematics of change. Whenever we want to understand how a quantity grows, decays, or evolves over time, we study its rate of change. Naturally, mathematicians began asking the same question about exponential functions.

Consider a general exponential function $a^x$. Calculus shows that

$$
\frac{d}{dx}a^x=a^x\ln a.
$$

Most exponential functions return with an extra factor attached. 
But when the base is exactly $e$, $\ln e=1$, and the formula becomes

$$
\frac{d}{dx}e^x=e^x.
$$

The function reproduces itself perfectly under differentiation. Among all exponential functions, it is the only one with this property. 

The number nobody was looking for had finally found its natural home.


## $e$ Is Everywhere
The special derivative property of $e$ would be interesting on its own, but its real importance comes from the way many natural processes behave.

In many situations, the rate at which something changes depends on how much of it already exists. A larger population produces more births. A larger investment earns more interest. A larger quantity of radioactive material produces more decay events.

Calculus describes these situations using differential equations, and the solutions repeatedly involve the exponential function $e^x$.


As a result, the same number that appeared in logarithms, compound interest, and infinite series begins to appear throughout science.


This idea appears throughout science.

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

Napier wanted faster calculations. Bernoulli investigated compound interest. Euler connected seemingly unrelated discoveries into a single mathematical framework. Later, calculus revealed why the same number appears whenever change occurs continuously.

At every turn, mathematicians pursued different problems, each following their own line of inquiry. Yet the same constant kept appearing, surfacing again and again in their results.

The journey of $e$ spans astronomy, finance, logarithms, infinite series, and calculus. What makes this remarkable is not merely that the number appears in many places, but that these appearances were discovered independently before anyone realized they were connected.

That is what makes the story of $e$ unusual. It was not invented, designed, or chosen. It revealed itself gradually, appearing wherever the mathematics of growth, change, and accumulation was pushed far enough.
The number nobody was looking for had been there all along.
