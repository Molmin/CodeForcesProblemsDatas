## Description

<div><p>Petya has a string of length <span class="tex-span"><i>n</i></span> consisting of small and large English letters and digits.</p><p>He performs <span class="tex-span"><i>m</i></span> operations. Each operation is described with two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> and a character <span class="tex-span"><i>c</i></span>: Petya removes from the string all characters <span class="tex-span"><i>c</i></span> on positions between <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>, inclusive. It's obvious that the length of the string remains the same or decreases after each operation.</p><p>Find how the string will look like after Petya performs all <span class="tex-span"><i>m</i></span> operations.</p></div><div class="input-specification"><p>The first string contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the length of the string and the number of operations.</p><p>The second line contains the string of length <span class="tex-span"><i>n</i></span>, consisting of small and large English letters and digits. Positions in the string are enumerated from <span class="tex-span">1</span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i></span>), followed by a character <span class="tex-span"><i>c</i></span>, which is a small or large English letter or a digit. This line describes one operation. It is guaranteed that <span class="tex-span"><i>r</i></span> doesn't exceed the length of the string <span class="tex-span"><i>s</i></span> before current operation.</p></div><div class="output-specification"><p>Print the string Petya will obtain after performing all <span class="tex-span"><i>m</i></span> operations. If the strings becomes empty after all operations, print an empty line.</p></div>

## Input

<p>The first string contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the length of the string and the number of operations.</p><p>The second line contains the string of length <span class="tex-span"><i>n</i></span>, consisting of small and large English letters and digits. Positions in the string are enumerated from <span class="tex-span">1</span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i></span>), followed by a character <span class="tex-span"><i>c</i></span>, which is a small or large English letter or a digit. This line describes one operation. It is guaranteed that <span class="tex-span"><i>r</i></span> doesn't exceed the length of the string <span class="tex-span"><i>s</i></span> before current operation.</p>

## Output

<p>Print the string Petya will obtain after performing all <span class="tex-span"><i>m</i></span> operations. If the strings becomes empty after all operations, print an empty line.</p>





```input1
4 2
abac
1 3 a
2 2 c

```




```input2
3 2
A0z
1 3 0
1 1 z

```




```input3
10 4
agtFrgF4aF
2 5 g
4 9 F
1 5 4
1 7 a

```




```input4
9 5
aAAaBBccD
1 4 a
5 6 c
2 3 B
4 4 D
2 3 A

```




```output1
b

```




```output2
Az

```




```output3
tFrg4

```




```output4
AB

```



## Note

<p>In the first example during the first operation both letters '<span class="tex-font-style-tt">a</span>' are removed, so the string becomes "<span class="tex-font-style-tt">bc</span>". During the second operation the letter '<span class="tex-font-style-tt">c</span>' (on the second position) is removed, and the string becomes "<span class="tex-font-style-tt">b</span>".</p><p>In the second example during the first operation Petya removes '<span class="tex-font-style-tt">0</span>' from the second position. After that the string becomes "<span class="tex-font-style-tt">Az</span>". During the second operations the string doesn't change.</p>
