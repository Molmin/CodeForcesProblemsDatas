## Description

<div><p>One day little Vasya found mom's pocket book. The book had <span class="tex-span"><i>n</i></span> names of her friends and unusually enough, each name was exactly <span class="tex-span"><i>m</i></span> letters long. Let's number the names from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order in which they are written.</p><p>As mom wasn't home, Vasya decided to play with names: he chose three integers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>i</i> &lt; <i>j</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>m</i></span>), then he took names number <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> and swapped their prefixes of length <span class="tex-span"><i>k</i></span>. For example, if we take names "<span class="tex-font-style-tt">CBDAD</span>" and "<span class="tex-font-style-tt">AABRD</span>" and swap their prefixes with the length of <span class="tex-span">3</span>, the result will be names "<span class="tex-font-style-tt">AABAD</span>" and "<span class="tex-font-style-tt">CBDRD</span>".</p><p>You wonder how many different names Vasya can write instead of name number <span class="tex-span">1</span>, if Vasya is allowed to perform any number of the described actions. As Vasya performs each action, he chooses numbers <span class="tex-span"><i>i</i></span>, <span class="tex-span"><i>j</i></span>, <span class="tex-span"><i>k</i></span> independently from the previous moves and his choice is based entirely on his will. The sought number can be very large, so you should only find it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of names and the length of each name, correspondingly. Then <span class="tex-span"><i>n</i></span> lines contain names, each name consists of exactly <span class="tex-span"><i>m</i></span> uppercase Latin letters.</p></div><div class="output-specification"><p>Print the single number — the number of different names that could end up in position number <span class="tex-span">1</span> in the pocket book after the applying the procedures described above. Print the number modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 100</span>) — the number of names and the length of each name, correspondingly. Then <span class="tex-span"><i>n</i></span> lines contain names, each name consists of exactly <span class="tex-span"><i>m</i></span> uppercase Latin letters.</p>

## Output

<p>Print the single number — the number of different names that could end up in position number <span class="tex-span">1</span> in the pocket book after the applying the procedures described above. Print the number modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
2 3
AAB
BAA

```




```input2
4 5
ABABA
BCGDG
AAAAA
YABSA

```




```output1
4

```




```output2
216

```



## Note

<p>In the first sample Vasya can get the following names in the position number <span class="tex-span">1</span>: "AAB", "AAA", "BAA" and "BAB".</p>
