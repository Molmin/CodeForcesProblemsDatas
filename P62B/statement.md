## Description

<div><p>Tyndex is again well ahead of the rivals! The reaction to the release of Zoozle Chrome browser was the release of a new browser Tyndex.Brome!</p><p>The popularity of the new browser is growing daily. And the secret is not even the Tyndex.Bar installed (the Tyndex.Bar automatically fills the glass with the finest 1664 cognac after you buy Tyndex.Bottles and insert in into a USB port). It is highly popular due to the well-thought interaction with the user.</p><p>Let us take, for example, the system of automatic address correction. Have you entered <span class="tex-font-style-tt">codehorses</span> instead of <span class="tex-font-style-tt">codeforces</span>? The gloomy Zoozle Chrome will sadly say that the address does not exist. Tyndex.Brome at the same time will automatically find the closest address and sent you there. That's brilliant!</p><p>How does this splendid function work? That's simple! For each potential address a function of the <span class="tex-span"><i>F</i></span> error is calculated by the following rules:</p><ul> <li> for every letter <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> from the potential address <span class="tex-span"><i>c</i></span> the closest position <span class="tex-span"><i>j</i></span> of the letter <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> in the address (<span class="tex-span"><i>s</i></span>) entered by the user is found. The absolute difference <span class="tex-span">|<i>i</i> - <i>j</i>|</span> of these positions is added to <span class="tex-span"><i>F</i></span>. So for every <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ |<i>c</i>|</span>) the position <span class="tex-span"><i>j</i></span> is chosen such, that <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> = <i>s</i><sub class="lower-index"><i>j</i></sub></span>, and <span class="tex-span">|<i>i</i> - <i>j</i>|</span> is minimal possible. </li><li> if no such letter <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> exists in the address entered by the user, then the length of the potential address <span class="tex-span">|<i>c</i>|</span> is added to <span class="tex-span"><i>F</i></span>. </li></ul><p>After the values of the error function have been calculated for all the potential addresses the most suitable one is found. </p><p>To understand the special features of the above described method better, it is recommended to realize the algorithm of calculating the <span class="tex-span"><i>F</i></span> function for an address given by the user and some set of potential addresses. Good luck!</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>). They are the number of potential addresses and the length of the address entered by the user. The next line contains <span class="tex-span"><i>k</i></span> lowercase Latin letters. They are the address entered by the user (<span class="tex-span"><i>s</i></span>). Each next <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) line contains a non-empty sequence of lowercase Latin letters. They are the potential address. It is guaranteed that the total length of all the lines does not exceed <span class="tex-span">2·10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>On each <span class="tex-span"><i>n</i></span> line of the output file print a single number: the value of the error function when the current potential address is chosen.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>). They are the number of potential addresses and the length of the address entered by the user. The next line contains <span class="tex-span"><i>k</i></span> lowercase Latin letters. They are the address entered by the user (<span class="tex-span"><i>s</i></span>). Each next <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) line contains a non-empty sequence of lowercase Latin letters. They are the potential address. It is guaranteed that the total length of all the lines does not exceed <span class="tex-span">2·10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>On each <span class="tex-span"><i>n</i></span> line of the output file print a single number: the value of the error function when the current potential address is chosen.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>





```input1
2 10
codeforces
codeforces
codehorses

```




```input2
9 9
vkontakte
vcontacte
vkontrakte
vkollapse
vkrokodile
vtopke
vkapuste
vpechke
vk
vcodeforcese

```




```output1
0
12

```




```output2
18
14
36
47
14
29
30
0
84

```


