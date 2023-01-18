## Description

<div><p>The Little Elephant loves strings very much. </p><p>He has an array <span class="tex-span"><i>a</i></span> from <span class="tex-span"><i>n</i></span> strings, consisting of lowercase English letters. Let's number the elements of the array from 1 to <span class="tex-span"><i>n</i></span>, then let's denote the element number <span class="tex-span"><i>i</i></span> as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. For each string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span> the Little Elephant wants to find the number of pairs of integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>a</i><sub class="lower-index"><i>i</i></sub>|)</span> such that substring <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>[<i>l</i>... <i>r</i>]</span> is a substring to at least <span class="tex-span"><i>k</i></span> strings from array <span class="tex-span"><i>a</i></span> (including the <span class="tex-span"><i>i</i></span>-th string).</p><p>Help the Little Elephant solve this problem.</p><p>If you are not familiar with the basic notation in string problems, you can find the corresponding definitions in the notes.</p></div><div class="input-specification"><p>The first line contains two space-separated integers — <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Next <span class="tex-span"><i>n</i></span> lines contain array <span class="tex-span"><i>a</i></span>. The <span class="tex-span"><i>i</i></span>-th line contains a non-empty string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, consisting of lowercase English letter. The total length of all strings <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>On a single line print <span class="tex-span"><i>n</i></span> space-separated integers — the <span class="tex-span"><i>i</i></span>-th number is the answer for string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Please, do not use the %lld specifier to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the %I64d specifier.</p></div>

## Input

<p>The first line contains two space-separated integers — <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup>)</span>. Next <span class="tex-span"><i>n</i></span> lines contain array <span class="tex-span"><i>a</i></span>. The <span class="tex-span"><i>i</i></span>-th line contains a non-empty string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, consisting of lowercase English letter. The total length of all strings <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>On a single line print <span class="tex-span"><i>n</i></span> space-separated integers — the <span class="tex-span"><i>i</i></span>-th number is the answer for string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Please, do not use the %lld specifier to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the %I64d specifier.</p>





```input1
3 1
abc
a
ab

```




```input2
7 4
rubik
furik
abab
baba
aaabbbababa
abababababa
zero

```




```output1
6 1 3 

```




```output2
1 0 9 9 21 30 0 

```



## Note

<p>Let's assume that you are given string <span class="tex-span"><i>a</i> = <i>a</i><sub class="lower-index">1</sub><i>a</i><sub class="lower-index">2</sub>... <i>a</i><sub class="lower-index">|<i>a</i>|</sub></span>, then let's denote the string's length as <span class="tex-span">|<i>a</i>|</span> and the string's <span class="tex-span"><i>i</i></span>-th character as <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>A substring <span class="tex-span"><i>a</i>[<i>l</i>... <i>r</i>]</span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>a</i>|)</span> of string <span class="tex-span"><i>a</i></span> is string <span class="tex-span"><i>a</i><sub class="lower-index"><i>l</i></sub><i>a</i><sub class="lower-index"><i>l</i> + 1</sub>... <i>a</i><sub class="lower-index"><i>r</i></sub></span>.</p><p>String <span class="tex-span"><i>a</i></span> is a substring of string <span class="tex-span"><i>b</i></span>, if there exists such pair of integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>l</i> ≤ <i>r</i> ≤ |<i>b</i>|)</span>, that <span class="tex-span"><i>b</i>[<i>l</i>... <i>r</i>] = <i>a</i></span>.</p>
