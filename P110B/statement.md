## Description

<div><p><span class="tex-font-style-underline">Petya loves lucky numbers. We all know that lucky numbers are the positive integers whose decimal representations contain only the lucky digits <span class="tex-font-style-bf">4</span> and <span class="tex-font-style-bf">7</span>. For example, numbers <span class="tex-font-style-bf">47</span>, <span class="tex-font-style-bf">744</span>, <span class="tex-font-style-bf">4</span> are lucky and <span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">17</span>, <span class="tex-font-style-bf">467</span> are not.</span></p><p>Petya recently learned to determine whether a string of lowercase Latin letters is lucky. For each individual letter all its positions in the string are written out in the increasing order. This results in <span class="tex-span">26</span> lists of numbers; some of them can be empty. A string is considered lucky if and only if in each list the absolute difference of any two <span class="tex-font-style-bf">adjacent</span> numbers is a lucky number. </p><p>For example, let's consider string "<span class="tex-font-style-tt">zbcdzefdzc</span>". The lists of positions of equal letters are:</p><ul><li> <span class="tex-font-style-tt">b</span>: <span class="tex-span">2</span></li><li> <span class="tex-font-style-tt">c</span>: <span class="tex-span">3, 10</span></li><li> <span class="tex-font-style-tt">d</span>: <span class="tex-span">4, 8</span></li><li> <span class="tex-font-style-tt">e</span>: <span class="tex-span">6</span></li><li> <span class="tex-font-style-tt">f</span>: <span class="tex-span">7</span></li><li> <span class="tex-font-style-tt">z</span>: <span class="tex-span">1, 5, 9</span></li><li> Lists of positions of letters <span class="tex-font-style-tt">a</span>, <span class="tex-font-style-tt">g</span>, <span class="tex-font-style-tt">h</span>, ..., <span class="tex-font-style-tt">y</span> are empty.</li></ul><p>This string is lucky as all differences are lucky numbers. For letters <span class="tex-font-style-tt">z</span>: <span class="tex-span">5 - 1 = 4</span>, <span class="tex-span">9 - 5 = 4</span>, for letters <span class="tex-font-style-tt">c</span>: <span class="tex-span">10 - 3 = 7</span>, for letters <span class="tex-font-style-tt">d</span>: <span class="tex-span">8 - 4 = 4</span>. </p><p>Note that if some letter occurs only once in a string, it doesn't influence the string's luckiness after building the lists of positions of equal letters. The string where all the letters are distinct is considered lucky.</p><p>Find the lexicographically minimal lucky string whose length equals <span class="tex-span"><i>n</i></span>.</p></div><div class="input-specification"><p>The single line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of the sought string.</p></div><div class="output-specification"><p>Print on the single line the lexicographically minimal lucky string whose length equals <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The single line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the length of the sought string.</p>

## Output

<p>Print on the single line the lexicographically minimal lucky string whose length equals <span class="tex-span"><i>n</i></span>.</p>





```input1
5

```




```input2
3

```




```output1
abcda

```




```output2
abc

```



## Note

<p>The lexical comparison of strings is performed by the &lt; operator in modern programming languages. String <span class="tex-span"><i>a</i></span> is lexicographically less than string <span class="tex-span"><i>b</i></span> if exists such <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>b</i><sub class="lower-index"><i>i</i></sub></span>, and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> = <i>b</i><sub class="lower-index"><i>j</i></sub></span>.</p>
