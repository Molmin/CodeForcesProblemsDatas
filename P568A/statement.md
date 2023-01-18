## Description

<div><p>Rikhail Mubinchik believes that the current definition of prime numbers is obsolete as they are too complex and unpredictable. A palindromic number is another matter. It is aesthetically pleasing, and it has a number of remarkable properties. Help Rikhail to convince the scientific community in this!</p><p>Let us remind you that a number is called <span class="tex-font-style-it">prime</span> if it is integer larger than one, and is not divisible by any positive integer other than itself and one.</p><p>Rikhail calls a number a <span class="tex-font-style-it">palindromic</span> if it is integer, positive, and its decimal representation without leading zeros is a palindrome, i.e. reads the same from left to right and right to left.</p><p>One problem with prime numbers is that there are too many of them. Let's introduce the following notation: <span class="tex-span">π(<i>n</i>)</span>&nbsp;— the number of primes no larger than <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>rub</i>(<i>n</i>)</span>&nbsp;— the number of palindromic numbers no larger than <span class="tex-span"><i>n</i></span>. Rikhail wants to prove that there are a lot more primes than palindromic ones.</p><p>He asked you to solve the following problem: for a given value of the coefficient <span class="tex-span"><i>A</i></span> find the maximum <span class="tex-span"><i>n</i></span>, such that <span class="tex-span">π(<i>n</i>) ≤ <i>A</i>·<i>rub</i>(<i>n</i>)</span>.</p></div><div class="input-specification"><p>The input consists of two positive integers <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>q</i></span>, the numerator and denominator of the fraction that is the value of <span class="tex-span"><i>A</i></span>&nbsp;(<img align="middle" class="tex-formula" src="file://frHPWDW5.png" style="max-width: 100.0%;max-height: 100.0%;">,&nbsp;<img align="middle" class="tex-formula" src="file://ii1sK0CN.png" style="max-width: 100.0%;max-height: 100.0%;">).</p></div><div class="output-specification"><p>If such maximum number exists, then print it. Otherwise, print <span class="tex-font-style-tt">"Palindromic tree is better than splay tree"</span> (without the quotes).</p></div>

## Input

<p>The input consists of two positive integers <span class="tex-span"><i>p</i></span>, <span class="tex-span"><i>q</i></span>, the numerator and denominator of the fraction that is the value of <span class="tex-span"><i>A</i></span>&nbsp;(<img align="middle" class="tex-formula" src="file://frHPWDW5.png" style="max-width: 100.0%;max-height: 100.0%;">,&nbsp;<img align="middle" class="tex-formula" src="file://ii1sK0CN.png" style="max-width: 100.0%;max-height: 100.0%;">).</p>

## Output

<p>If such maximum number exists, then print it. Otherwise, print <span class="tex-font-style-tt">"Palindromic tree is better than splay tree"</span> (without the quotes).</p>





```input1
1 1

```




```input2
1 42

```




```input3
6 4

```




```output1
40

```




```output2
1

```




```output3
172

```


