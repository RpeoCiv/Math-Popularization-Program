### Mathematical induction

###### Auther:Czhuman

How do you go about understanding mathematical induction?In fact, it can be summarized as a domino process, to push down a row of dominoes, first of all, they must be laid out in the shape of one of the fall behind all will fall, and then deduce the most beginning of the one.

Let's take a simple example of Gaussian summation:

You have a money jar in front of you
On the first day, you put one dollar in the jar, and there is one dollar in the jar
On the second day, you put in two dollars, there are 1+2=3 dollars in the jar
On the third day, you put in three dollars, there are 1+2+3=6 dollars in the jar

Continuously continue, so how much do you have on the nth day?

In fact it can be done the dumb way, starting with 1, 1+2+3+4+... +n

But is this too stupid?

I'm sure you've all read the short story about the Gaussian calculation of this problem. In the story, Gauss uses a formula of (n+1)*n/2 for the final solution.

Next we try to analyze

First, Gauss applies the following equation
$$
1+2+3+...+100=\frac{100(100+1)}{2}
$$
Then substitute the variable n
$$
1+2+3+...+n=\frac{n(n+1)}{2}
$$
So, how do we prove that this number is possible for any n?

The next step is to use mathematical induction.

##### A few examples

Let's look at a few simple examples to understand mathematical induction

We define a function A(n)
$$
A(n)=2n\quad(n\in \N)
$$
So, is this function even for any n that satisfies the condition?

The answer is obvious, any positive integer multiplied by 2 gives an even number, so this proposition is true.

We again define a function B(n)
$$
B(n)=3n\quad(n\in \N)
$$
We again assume that for any n we can obtain the odd number.

It is clear that this proposition is disproved when n equals 2, and is therefore not valid.

Next we look at Gauss's inference
$$
\sum_{i=1}^ni=\frac{n(n+1)}{2}\quad(n\in \N)
$$
We then need to use mathematical induction to prove that this holds.

First, before proceeding with this step, I think it is necessary to perform some precise definitions of mathematical induction

Mathematical induction is a way to prove whether a proposition holds for all natural numbers

Now to prove that n in P(n) holds for any natural number

There are two overall steps.

1. prove that P(0) holds
2. Prove that if P(k) holds regardless of the natural number k, then P(k+1) also holds

We will make the first step the substrate and the second step the induction

Let's start proving it

Define the proposition G(n)
$$
G(n)=1+2+3+...+n=\frac{n(n+1)}{2}
$$
Start the first step: prove the substrate
$$
G(0)=\frac{0(0+1)}{2}=0
$$
can be proved by direct arithmetic

Second step, induction

First we define an equation that is assumed to hold
$$
G(k)=1+2+3+...+k=\frac{k(k+1)}{2}
$$
Next, prove that G(k+1) holds
$$
1+2+3+...+k+(k+1)=\frac{(k+1)((k+1)+1)}{2}
$$
Take the left side out for separate discussion
$$
\begin{align}
left&=1+2+3+...+k+(k+1)\\
&=\frac{k(k+1)}{2}+(k+1)\quad 1+2+3+...+k=\frac{k(k+1)}{2}\\
&=\frac{k(k+1)}{2}+\frac{2(k+1)}{2}\\
&=\frac{k(k+1)+2(k+1)}{2}\\
&=\frac{(k+2)(k+1)}{2}
\end{align}
$$
Next look at the right side
$$
\begin{align}
right&=\frac{(k+1)((k+1)+1)}{2}\\
&=\frac{(k+1)(k+2)}{2}
\end{align}
$$
We can then find that the left and right sides are equal

So now that you've mastered basic mathematical induction, now start trying to prove that 1+2+3+... +n=n^2 as an exercise!

