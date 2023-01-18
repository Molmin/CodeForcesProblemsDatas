## Description

<div><p>Polycarpus has <span class="tex-span"><i>t</i></span> safes. The password for each safe is a square matrix consisting of decimal digits '<span class="tex-font-style-tt">0</span>' ... '<span class="tex-font-style-tt">9</span>' (the sizes of passwords to the safes may vary). Alas, Polycarpus has forgotten all passwords, so now he has to restore them.</p><p>Polycarpus enjoys prime numbers, so when he chose the matrix passwords, he wrote a prime number in each row of each matrix. To his surprise, he found that all the matrices turned out to be symmetrical (that is, they remain the same after transposition). Now, years later, Polycarp was irritated to find out that he remembers only the prime numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>, written in the first lines of the password matrices.</p><p>For each safe find the number of matrices which can be passwords to it.</p><p>The number of digits in <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> determines the number of rows and columns of the <span class="tex-span"><i>i</i></span>-th matrix. One prime number can occur in several rows of the password matrix or in several matrices. The prime numbers that are written not in the first row of the matrix may have leading zeros.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 30</span>) — the number of safes. Next <span class="tex-span"><i>t</i></span> lines contain integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">10 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 99999</span>), <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is a prime number written in the first row of the password matrix for the <span class="tex-span"><i>i</i></span>-th safe. All <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>'s are written without leading zeros.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>t</i></span> numbers, the <span class="tex-span"><i>i</i></span>-th of them should be the number of matrices that can be a password to the <span class="tex-span"><i>i</i></span>-th safe. Print the numbers on separate lines.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 30</span>) — the number of safes. Next <span class="tex-span"><i>t</i></span> lines contain integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">10 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 99999</span>), <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is a prime number written in the first row of the password matrix for the <span class="tex-span"><i>i</i></span>-th safe. All <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>'s are written without leading zeros.</p>

## Output

<p>Print <span class="tex-span"><i>t</i></span> numbers, the <span class="tex-span"><i>i</i></span>-th of them should be the number of matrices that can be a password to the <span class="tex-span"><i>i</i></span>-th safe. Print the numbers on separate lines.</p>





```input1
4
11
239
401
9001

```




```output1
4
28
61
2834

```



## Note

<p>Here is a possible password matrix for the second safe: </p><pre class="verbatim"><br>239<br>307<br>977<br></pre><p>Here is a possible password matrix for the fourth safe: </p><pre class="verbatim"><br>9001<br>0002<br>0002<br>1223 <br></pre>
