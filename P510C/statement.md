## Description

<div><p>Fox Ciel is going to publish a paper on FOCS (Foxes Operated Computer Systems, pronounce: "Fox"). She heard a rumor: the authors list on the paper is always sorted in the <span class="tex-font-style-underline">lexicographical</span> order. </p><p>After checking some examples, she found out that sometimes it wasn't true. On some papers authors' names weren't sorted in <span class="tex-font-style-underline">lexicographical</span> order in normal sense. But it was always true that after some modification of the order of letters in alphabet, the order of authors becomes <span class="tex-font-style-underline">lexicographical</span>!</p><p>She wants to know, if there exists an order of letters in Latin alphabet such that the names on the paper she is submitting are following in the <span class="tex-font-style-underline">lexicographical</span> order. If so, you should find out any such order.</p><p><span class="tex-font-style-underline">Lexicographical</span> order is defined in following way. When we compare <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>, first we find the leftmost position with differing characters: <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> ≠ <i>t</i><sub class="lower-index"><i>i</i></sub></span>. If there is no such position (i. e. <span class="tex-span"><i>s</i></span> is a prefix of <span class="tex-span"><i>t</i></span> or vice versa) the shortest string is less. Otherwise, we compare characters <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> according to their order in alphabet.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>): number of names.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contain one string <span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ |<i>name</i><sub class="lower-index"><i>i</i></sub>| ≤ 100</span>), the <span class="tex-span"><i>i</i></span>-th name. Each name contains only lowercase Latin letters. All names are different.</p></div><div class="output-specification"><p>If there exists such order of letters that the given names are sorted lexicographically, output any such order as a permutation of characters 'a'–'z' (i. e. first output the first letter of the modified alphabet, then the second, and so on).</p><p>Otherwise output a single word "Impossible" (without quotes).</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>): number of names.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines contain one string <span class="tex-span"><i>name</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ |<i>name</i><sub class="lower-index"><i>i</i></sub>| ≤ 100</span>), the <span class="tex-span"><i>i</i></span>-th name. Each name contains only lowercase Latin letters. All names are different.</p>

## Output

<p>If there exists such order of letters that the given names are sorted lexicographically, output any such order as a permutation of characters 'a'–'z' (i. e. first output the first letter of the modified alphabet, then the second, and so on).</p><p>Otherwise output a single word "Impossible" (without quotes).</p>





```input1
3
rivest
shamir
adleman

```




```input2
10
tourist
petr
wjmzbmr
yeputons
vepifanov
scottwu
oooooooooooooooo
subscriber
rowdark
tankengineer

```




```input3
10
petr
egor
endagorion
feferivan
ilovetanyaromanova
kostka
dmitriyh
maratsnowbear
bredorjaguarturnik
cgyforever

```




```input4
7
car
care
careful
carefully
becarefuldontforgetsomething
otherwiseyouwillbehacked
goodluck

```




```output1
bcdefghijklmnopqrsatuvwxyz

```




```output2
Impossible

```




```output3
aghjlnopefikdmbcqrstuvwxyz

```




```output4
acbdefhijklmnogpqrstuvwxyz

```


