# Special Numbers: Triangular, Oblong, Perfect, Deficient and Aboundant

## Triangular Numbers

*Triangular numbers* are those number that can be written as the sum of a consecutives series of numbers beginning whit 1. In general:

{{< katex display >}}
T_n = 1 + 2 + \dots + (n - 1) + n
{{< /katex >}}

The triangular numbers are given by the following explicit formulas

{{< katex display >}}
T_n = \sum_{k=1}^{n}k = 1 + 2 + \dots + n = \frac{n(n + 1)}{2}  
{{< /katex >}}

The sum of any two consecutive trriangular number is a square. This is is expressed b thee formula

{{< katex display >}}
T_n + T_{n-1} = n^2
{{< /katex >}}

## Oblong Numbers and Squares

A positive integer inthe form {{< katex >}}n(n+1){{< /katex >}} is called *oblong*. The *n*th oblong number is the sum of the first *n* even numbers:

{{< katex display >}}
2 + 4 + \dots + 2n = 2\frac{n(n+1)}{2} = n(n+1)
{{< /katex >}}

The sum of the first *n* odd numbers is

{{< katex display >}}
1 + 3 + \dots + (2n-1) = \sum_{k=1}^{n}(2k-1) = 2(1 + 2 + \dots + n) - n = 2\frac{n(n+1)}{2} - n = n^2
{{< /katex >}}

Let {{< katex >}}S = 1 + a + a^2 + a^3 + \dots + a^{n-1}{{< /katex >}}, with {{< katex >}}a \in \mathbb{N}{{< /katex >}}. Then {{< katex >}}aS = a + a^2 + \dots + a^{n-a} + a^n{{< /katex >}}. Subtract the first equation from the second and we get {{< katex >}}(a - 1)S = a^{n-1}{{< /katex >}}, and so

{{< katex display >}}
\sum_{i=0}^{n} a^i = 1 + a + a^2 + \dots + a^{n-1} = \frac{a^n-1}{a-1}
{{< /katex >}}

In this way the Pythagoreans computed the sum of the first *n* powers of two: {{< katex >}}\sum_{i=0}^{n-1}2^i = 2^{n}-1{{< /katex >}}.

## Deficient, Abundant and Perfect numbers

If the sum of the proper factors of *n* is less than *n*, then *n* is *deficeint*. If the sum of the proper factors of *n* exeeds *n*, then *n* is *abundant*. If the sum of th proper factor of *n* is equal to *n*, then *n* is *perfect*. See [wiki](https://en.wikipedia.org/wiki/Perfect_number) for more infos.

It is not know today if there are infinitely many perfec numbers, and all the perfect numbers are even, no one knows if there are any odd perfect numbers!

The smallest abundant odd number is *945*, while the smallest aboundant even number is *12*.

Leonhard Euler showed that all the *even* perfect numbers are of the form {{< katex >}}2^{n-1}(2^n-1){{< /katex >}} where {{< katex >}}2^n-1{{< /katex >}} is prime.

The prime sum {{< katex >}}2^n-1{{< /katex >}} is called *Mersenne prime*.

*Amicable numbers* are two different numbers related in such a way that the sum of the proper divisors of each is equal to the other number.

The smallest pair of amicable numbers is {{< katex >}}(220, 284){{< /katex >}}. They are amicable because the proper divisors of {{< katex >}}220{{< /katex >}} are {{< katex >}}1, 2, 4, 5, 10, 11, 20, 22, 44, 55{{< /katex >}} and {{< katex >}}110{{< /katex >}}, of which the sum is {{< katex >}}284{{< /katex >}}; and the proper divisors of {{< katex >}}284{{< /katex >}} are {{< katex >}}1, 2, 4, 71{{< /katex >}} and {{< katex >}}142{{< /katex >}}, of which the sum is {{< katex >}}220{{< /katex >}}.
