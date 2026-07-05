



# Chapter 5

## Why Calculus Loves $e$

## The Only Exponential Function That Reproduces Itself

By now, we have seen that $e$ is very good at showing up uninvited.

Astronomers wanted faster calculations, and something related to $e$ was hiding in the background.
Napier invented logarithms, and $e$ quietly slipped into the machinery.
Bernoulli studied compound interest, and $e$ appeared again.
Euler connected the clues and realized:

> “Wait a minute. This number keeps coming back.”

But up to this point, $e$ was still just a mysterious number that appeared in several unexpected places.

What truly made it the **natural base** was calculus.

Calculus is not mainly about things that sit still.
It is about change.

How does the position of an object change?
How does a population grow?
How does money accumulate?
How does a radioactive substance decay?
How does voltage fall in a circuit?

Whenever a problem involves a **rate of change**, calculus walks into the room.

And this is exactly where $e$ becomes special.

It is the number that seems designed for continuous change.

---


Let us begin with a general exponential function:

$$
a^x
$$

Here, $a$ is the base.

If $a=2$, we get:

$$
2^x
$$

If $a=10$, we get:

$$
10^x
$$

If $a=e$, we get:

$$
e^x
$$

At first, these all look like ordinary exponential functions.
They all grow.
They simply grow at different speeds.

But calculus asks a sharper question:

> What is the rate of change of this function?

In other words, calculus asks for the derivative.

For a general exponential function, we have:

$$
\frac{d}{dx}a^x=a^x\ln a
$$

This means that the derivative of $a^x$ is still related to $a^x$, but it comes with an extra factor:

$$
\ln a
$$

For example:

$$
\frac{d}{dx}2^x=2^x\ln2
$$

and:

$$
\frac{d}{dx}10^x=10^x\ln10
$$

Both functions survive differentiation, but they come back wearing a little mathematical backpack.

That backpack is $\ln a$.

But when the base is exactly $e$, something remarkable happens:

$$
\ln e=1
$$

So:

$$
\frac{d}{dx}e^x=e^x
$$

That is extraordinary.

The rate of change of $e^x$ is exactly itself.

Unlike $2^x$, it does not need to be multiplied by $\ln2$.
Unlike $10^x$, it does not need to carry around $\ln10$.
It simply says:

> “Differentiate me if you want. I will still be myself.”

This is the central reason why $e^x$ is so important in calculus.

Among all exponential functions, it is the only one whose derivative is exactly the same as the original function.

![Tangent line visualization](./e_natural_base_assets/tangent_line_visualization.png)

The image above shows the tangent line to $y=e^x$ at $x=0$.

When $x=0$:

$$
e^0=1
$$

So the curve passes through the point:

$$
(0,1)
$$

Since:

$$
\frac{d}{dx}e^x=e^x
$$

the slope at $x=0$ is also:

$$
e^0=1
$$

Therefore, the tangent line at that point is:

$$
y=x+1
$$

This is one of the beautiful features of $e^x$:

At the point $(0,1)$, its height is $1$, and its slope is also $1$.

No one forced it to behave this way.
It simply does.

Other bases are less lucky.

For $2^x$, the slope at $x=0$ is:

$$
\ln2\approx0.693
$$

For $10^x$, the slope at $x=0$ is:

$$
\ln10\approx2.303
$$

Only $e^x$ has slope exactly:

$$
1
$$

at $x=0$.

![Derivative comparison graph](./e_natural_base_assets/derivative_comparison_graph.png)

Think of this graph as an interview for exponential functions.

Calculus asks:

> “Can you remain exactly the same after differentiation?”

$2^x$ says:

> “Almost. But I need a factor of $\ln2$.”

$10^x$ says:

> “I can do it too, but I need a factor of $\ln10$.”

Then $e^x$ walks in and says:

> “No extra factor needed. I am already the answer.”

And calculus replies:

> “Excellent. You are the natural base.”

Before we reveal why one particular base wins this contest, it helps to actually see what happens when the base changes.

The following short video works like a base slider.  
As the value of $a$ changes, the graph of

$$
y=a^x
$$

changes with it.

Pay attention to two things:

1. how quickly the curve rises;
2. what happens to the slope near $x=0$.

<video src="./base_slider_exponential_ax.mp4" controls width="800"></video>

The video shows that changing the base is not just a cosmetic choice.

When $a$ is small, the exponential curve grows more slowly.  
When $a$ is large, the curve rises much more sharply.  
Each base creates its own version of exponential growth.

But calculus is not only asking:

> “Which curve grows faster?”

It is asking a more precise question:

> “Which exponential function has a rate of change that matches itself exactly?”

That is where $e$ enters the story.


## Why This Matters

This is not only a pretty formula.

It matters because many real-world processes are described by rates of change.

For example, a population often does not grow by adding the same fixed number every year.
Instead, the larger the population already is, the faster it tends to grow.

If the rate of growth is proportional to the current amount, we can write:

$$
\frac{dP}{dt}=rP
$$

This means:

The rate of change of the population $P$ is equal to the current population multiplied by a growth rate $r$.

The solution to this differential equation is:

$$
P(t)=P_0e^{rt}
$$

And there it is again.

$e$ appears not because mathematicians invited it, but because continuous growth naturally leads to it.

---

## $e$ Is Everywhere

### 1. Population Growth

If a population follows a continuous growth model, it can be written as:

$$
P(t)=P_0e^{rt}
$$

Here:

* $P_0$ is the initial population;
* $r$ is the growth rate;
* $t$ is time;
* $P(t)$ is the population after time $t$.

This does not mean that populations always grow this way forever.
Real populations are affected by food, space, disease, policy, climate, and many other factors.

But the formula captures a basic idea:

> The larger the current amount, the faster the absolute growth.

That is why $e$ appears.

---

### 2. Radioactive Decay

Radioactive decay looks like the opposite of population growth.

Population growth increases.
Radioactive decay decreases.

But mathematically, the structure is very similar.

If the amount of a radioactive substance is $N(t)$, then a common decay model is:

$$
N(t)=N_0e^{-\lambda t}
$$

Here:

* $N_0$ is the initial amount;
* $\lambda$ is the decay constant;
* $t$ is time;
* $N(t)$ is the amount remaining after time $t$.

The negative sign in the exponent:

$$
-\lambda t
$$

tells us that the quantity is decreasing rather than increasing.

But the key idea is the same:

> The rate of decay is proportional to the amount currently remaining.

The more material remains, the faster it decays.
The less material remains, the slower the decay becomes.

So $e$ appears again.

---

### 3. Electricity

In electricity, especially in an RC circuit made from a resistor and a capacitor, $e$ appears once more.

When a capacitor discharges, its voltage does not instantly fall to zero.
It decreases gradually.
At first, it drops quickly.
Later, it drops more slowly.

This kind of change can be modeled by exponential decay:

$$
V(t)=V_0e^{-t/RC}
$$

Here:

* $V_0$ is the initial voltage;
* $R$ is resistance;
* $C$ is capacitance;
* $t$ is time;
* $V(t)$ is the voltage after time $t$.

This shows that $e$ is not trapped inside textbooks.

It appears in physics, circuits, engineering, and the real behavior of changing systems.

The number that looks cold and abstract in a formula is quietly doing practical work in the real world.

---

## The Real Meaning of “Natural”

Now we can answer a very reasonable question:

Why is $e$ called the natural base?

Why not base $10$?

After all, base $10$ feels very familiar.

We count using:

$$
1,2,3,4,5,6,7,8,9,10
$$

Money is often written in decimal notation.
Measurements are often organized in powers of ten.
So base $10$ seems natural to us.

But here is the problem:

Base $10$ is natural to humans.
That does not mean it is natural to nature.

We probably use base $10$ largely because humans have ten fingers.
If humans had eight fingers, perhaps base $8$ would feel perfectly normal.

So why not base $2$?

Computers love base $2$.
In the binary world, $0$ and $1$ can build enormous systems.

But base $2$ is convenient for computers.
It was not chosen by continuous change itself.

Then why not base $7$?

Honestly, base $7$ has done nothing wrong.
It simply did not get the leading role in calculus.

What makes $e$ natural is this:

When mathematicians study continuous growth, decay, rates of change, and differential equations, $e$ appears again and again without being artificially chosen.

Human beings choose base $10$.
Computers use base $2$.
But continuous change keeps producing base $e$.

That is the real meaning of “natural.”

It is not natural because it looks simple.
In fact:

$$
2.718281828\cdots
$$

does not look simple at all.

It is natural because it belongs to the mathematics of change.

---

### 1. Mathematics

In mathematics, especially in calculus and analysis:

$$
\ln x
$$

usually means the natural logarithm, that is:

$$
\ln x=\log_e x
$$

In some mathematics textbooks, $\log x$ may also mean the natural logarithm.

So in many mathematical contexts:

$$
\log x=\ln x
$$

This feels natural to mathematicians because $e$ is the standard base for continuous change.

---

### 2. Engineering

In engineering, physics experiments, signal processing, and measurement contexts, $\log x$ often means the base-$10$ logarithm:

$$
\log x=\log_{10}x
$$

This appears often in decibels, orders of magnitude, and measurement scales.

That convention is connected to practical measurement habits.

---

### 3. Computer Science

In computer science, especially in algorithm analysis, $\log x$ is often associated with base $2$.

Binary search, binary trees, information coding, and digital systems are all closely related to powers of two.

So in these contexts, $\log n$ is often understood as:

$$
\log_2 n
$$

However, in Big-O notation, the base usually does not matter very much.

Different logarithm bases differ only by a constant factor.

For example:

$$
\log_2 n=\frac{\ln n}{\ln2}
$$

Since constant factors are ignored in Big-O notation, computer scientists often simply write:

$$
O(\log n)
$$

without specifying the base.

So when you see $\log x$, do not panic.

It is not trying to personally attack you.
It just has different social habits in different academic fields.

The safest method is simple:

Check the context.
Check the textbook.
Check the teacher’s definition.

And if you are writing it yourself, state the base clearly when needed.

Mathematics will not be offended by clarity.




# Conclusion

## The Number That Never Left

At the beginning of this story, nobody was searching for $e$.

There was no grand announcement.
No ancient mathematician stood on a mountain and declared:

> “Behold! I have found the natural base of the universe!”

The story began in a much less dramatic place:

people were tired of doing arithmetic.

Astronomers needed to calculate the positions of planets and stars.
Navigators needed reliable tables to guide ships across the sea.
Scientists needed ways to handle large numbers without spending their entire lives trapped inside multiplication.

So the first problem was not philosophical.

It was practical.

People were not asking:

> “What is the deepest number hidden inside continuous change?”

They were asking something much more human:

> “Can we please make these calculations less painful?”

That need led to logarithms.

John Napier did not invent logarithms because he was hunting for $e$.
His goal was to create a shortcut.
If multiplication could be turned into addition, then huge calculations would become faster, safer, and less exhausting.

Logarithms became a kind of pre-digital calculator.

For centuries, they helped astronomers, engineers, scientists, and students survive large computations.
But hidden inside the structure of logarithms was a number that had not yet fully revealed itself.

That number was $e$.

Then the story moved from the stars to the bank.

Jacob Bernoulli studied compound interest and asked what would happen if interest were compounded more and more frequently.

Once per year gave one result.
Four times per year gave a larger result.
Monthly, daily, hourly, every second — the more often the interest was compounded, the more the final amount increased.

But it did not increase forever.

Instead, it approached a limit:

$$
\left(1+\frac{1}{n}\right)^n
$$

As $n$ becomes larger and larger, this expression approaches:

$$
e \approx 2.71828
$$

So a number that had been hiding in logarithms appeared again in a completely different setting: compound interest.

At this point, the story had become suspicious.

Astronomy had pointed toward it.
Logarithms had contained it.
Banking had rediscovered it.

It was as if the same number kept walking into different rooms wearing different disguises.

Then Euler entered the story.

Euler did not simply find a new number.
More importantly, he recognized a pattern.

He saw that the number emerging from logarithms, the number appearing in Bernoulli’s limit, and the number arising in infinite series were not separate mysteries.

They were the same mystery.

Euler helped bring this number into the center of mathematics and gave it the simple symbol we still use today:

$$
e
$$

From that point on, $e$ was no longer just a strange recurring value.

It had become a named mathematical object.

But the deepest reason for its importance appeared in calculus.

Calculus studies change.

And among all exponential functions, one function behaves in the most remarkable way:

$$
e^x
$$

Its derivative is itself:

$$
\frac{d}{dx}e^x=e^x
$$

This means that the rate of change of $e^x$ is exactly $e^x$ again.

Other exponential functions almost do this, but not quite.

For example:

$$
\frac{d}{dx}2^x=2^x\ln2
$$

and:

$$
\frac{d}{dx}10^x=10^x\ln10
$$

They need extra factors.

But $e^x$ needs nothing added.

It is the exponential function that reproduces itself under differentiation.

That is why calculus loves $e$.

And that is why $e$ became the natural base.

Not because humans chose it for convenience.
Not because it looked simple.
Not because it was named after Euler.
Not because it had better branding than other numbers.

It became natural because continuous change kept producing it.

When a population grows at a rate proportional to its current size, $e$ appears:

$$
P(t)=P_0e^{rt}
$$

When a radioactive substance decays at a rate proportional to how much remains, $e$ appears:

$$
N(t)=N_0e^{-\lambda t}
$$

When a capacitor discharges in a circuit, $e$ appears:

$$
V(t)=V_0e^{-t/RC}
$$

Again and again, the same pattern returns:

when the rate of change depends on the current amount, $e$ is nearby.

This is the real meaning of “natural.”

Base $10$ feels natural to humans because we count with ten fingers.
Base $2$ feels natural to computers because digital systems use zeros and ones.
But base $e$ belongs to the mathematics of continuous growth and decay.

It is not natural because we are used to it.

It is natural because the structure of change itself keeps asking for it.

So the history of $e$ is not the story of one person discovering one number in one moment.

It is the story of a number being recognized slowly.

First as a computational shadow.
Then as a limit in compound interest.
Then as a central object in Euler’s mathematics.
Then as the natural language of calculus.
Finally, as a number woven into growth, decay, electricity, probability, and the changing world.

At first, mathematicians might have asked:

> “Where did this number come from?”

But eventually, the better question became:

> “Why does it keep appearing everywhere?”

That is what makes $e$ so fascinating.

It was the number nobody was looking for.

But once mathematics learned how to see it, it seemed to have been there all along.
