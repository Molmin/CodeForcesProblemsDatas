## Description

<div><p><span class="tex-font-style-it">Author note: I think some of you might remember the problem "Two Melodies" from Eductational Codeforces Round 22. Now it's time to make it a bit more difficult!</span></p><p>Alice is a composer, and recently she had recorded two tracks that became very popular. Now she has got a lot of fans who are waiting for new tracks. </p><p>This time Alice wants to form four melodies for her tracks.</p><p>Alice has a sheet with <span class="tex-span"><i>n</i></span> notes written on it. She wants to take four such non-empty non-intersecting subsequences that all of them form a <span class="tex-font-style-it">melody</span> and sum of their lengths is maximal.</p><p><span class="tex-font-style-it">Subsequence is a sequence that can be derived from another sequence by deleting some elements without changing the order of the remaining elements.</span></p><p>Subsequence forms a melody when each two adjacent notes either differ by <span class="tex-font-style-tt">1</span> or are congruent modulo <span class="tex-font-style-tt">7</span>.</p><p>You should write a program which will calculate maximum sum of lengths of such four non-empty non-intersecting subsequences that all of them form a melody.</p></div><div class="input-specification"><p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 3000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — notes written on a sheet.</p></div><div class="output-specification"><p>Print maximum sum of lengths of such four non-empty non-intersecting subsequences that all of them form a melody.</p></div>

## Input

<p>The first line contains one integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 3000</span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> integer numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — notes written on a sheet.</p>

## Output

<p>Print maximum sum of lengths of such four non-empty non-intersecting subsequences that all of them form a melody.</p>





```input1
5
1 3 5 7 9

```




```input2
5
1 3 5 7 2

```




```output1
4

```




```output2
5

```



## Note

<p>In the first example it is possible to compose <span class="tex-span">4</span> melodies by choosing any <span class="tex-span">4</span> notes (and each melody will consist of only one note).</p><p>In the second example it is possible to compose one melody with <span class="tex-span">2</span> notes — <span class="tex-span">{1, 2}</span>. Remaining notes are used in other three melodies (one note per each melody).</p>
