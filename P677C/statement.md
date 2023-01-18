## Description

<div><p>While walking down the street Vanya saw a label "Hide&amp;Seek". Because he is a programmer, he used <span class="tex-span">&amp;</span> as a bitwise AND for these two words represented as a integers in base <span class="tex-span">64</span> and got new word. Now Vanya thinks of some string <span class="tex-span"><i>s</i></span> and wants to know the number of pairs of words of length <span class="tex-span">|<i>s</i>|</span> (length of <span class="tex-span"><i>s</i></span>), such that their bitwise AND is equal to <span class="tex-span"><i>s</i></span>. As this number can be large, output it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>To represent the string as a number in numeral system with base <span class="tex-span">64</span> Vanya uses the following rules:</p><ul> <li> digits from '<span class="tex-font-style-tt">0</span>' to '<span class="tex-font-style-tt">9</span>' correspond to integers from <span class="tex-span">0</span> to <span class="tex-span">9</span>; </li><li> letters from '<span class="tex-font-style-tt">A</span>' to '<span class="tex-font-style-tt">Z</span>' correspond to integers from <span class="tex-span">10</span> to <span class="tex-span">35</span>; </li><li> letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">z</span>' correspond to integers from <span class="tex-span">36</span> to <span class="tex-span">61</span>; </li><li> letter '<span class="tex-font-style-tt">-</span>' correspond to integer <span class="tex-span">62</span>; </li><li> letter '<span class="tex-font-style-tt">_</span>' correspond to integer <span class="tex-span">63</span>. </li></ul></div><div class="input-specification"><p>The only line of the input contains a single word <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100 000</span>), consisting of digits, lowercase and uppercase English letters, characters '<span class="tex-font-style-tt">-</span>' and '<span class="tex-font-style-tt">_</span>'.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of possible pairs of words, such that their bitwise AND is equal to string <span class="tex-span"><i>s</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The only line of the input contains a single word <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100 000</span>), consisting of digits, lowercase and uppercase English letters, characters '<span class="tex-font-style-tt">-</span>' and '<span class="tex-font-style-tt">_</span>'.</p>

## Output

<p>Print a single integer&nbsp;— the number of possible pairs of words, such that their bitwise AND is equal to string <span class="tex-span"><i>s</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
z

```




```input2
V_V

```




```input3
Codeforces

```




```output1
3

```




```output2
9

```




```output3
130653412

```



## Note

<p>For a detailed definition of bitwise AND we recommend to take a look in the corresponding article in Wikipedia.</p><p>In the first sample, there are <span class="tex-span">3</span> possible solutions: </p><ol> <li> <span class="tex-span"><i>z</i>&amp;_ = 61&amp;63 = 61 = <i>z</i></span> </li><li> <span class="tex-span">_&amp;<i>z</i> = 63&amp;61 = 61 = <i>z</i></span> </li><li> <span class="tex-span"><i>z</i>&amp;<i>z</i> = 61&amp;61 = 61 = <i>z</i></span> </li></ol>
