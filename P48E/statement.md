## Description

<div><p>Once upon a time in a kingdom far, far away… Okay, let’s start at the point where Ivan the Fool met Gorynych the Dragon. Ivan took out his magic sword and the battle began. First Gorynych had <span class="tex-span"><i>h</i></span> heads and <span class="tex-span"><i>t</i></span> tails. With each strike of the sword Ivan can either cut off several heads (from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, but not more than Gorynych has at the moment), or several tails (from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>, but not more than Gorynych has at the moment). At the same time, horrible though it seems, Gorynych the Dragon can also grow new heads and tails. And the number of growing heads and tails is determined uniquely by the number of heads or tails cut by the current strike. When the total number of heads and tails exceeds <span class="tex-span"><i>R</i></span>, Gorynych the Dragon strikes its final blow and destroys Ivan the Fool. That’s why Ivan aims to cut off all the dragon’s heads and tails as quickly as possible and win. The events can also develop in a third way: neither of the opponents can win over the other one and they will continue fighting forever.</p><p>The tale goes like this; easy to say, hard to do. Your task is to write a program that will determine the battle’s outcome. Consider that Ivan strikes consecutively. After each blow Gorynych grows a number of new heads and tails depending on the number of cut ones. Gorynych the Dragon is defeated if after the blow he loses all his heads and tails and can’t grow new ones. Ivan fights in the optimal way (fools are lucky), i.e. </p><ul> <li> if Ivan can win, he wins having struck the least number of blows; </li><li> if it is impossible to defeat Gorynych, but is possible to resist him for an infinitely long period of time, then that’s the strategy Ivan chooses; </li><li> if Gorynych wins in any case, Ivan aims to resist him for as long as possible. </li></ul></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>R</i></span> (<span class="tex-span">0 ≤ <i>h</i>, <i>t</i>, <i>R</i> ≤ 200</span>, <span class="tex-span">0 &lt; <i>h</i> + <i>t</i> ≤ <i>R</i></span>) which represent the initial numbers of Gorynych’s heads and tails and the largest total number of heads and tails with which Gorynych the Dragon does not yet attack. The next line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>). The next <span class="tex-span"><i>n</i></span> contain pairs of non-negative numbers "<span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>" which represent the number of heads and the number of tails correspondingly, that will grow if Gorynych has <span class="tex-span"><i>i</i></span> heads (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) cut. The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200</span>) and then — the description of Gorynych’s behavior when his tails are cut off in the format identical to the one described above. All the numbers in the input file do not exceed <span class="tex-span">200</span>. </p></div><div class="output-specification"><p>Print "Ivan" (without quotes) in the first line if Ivan wins, or "Zmey" (that means a dragon in Russian) if Gorynych the Dragon wins. In the second line print a single integer which represents the number of blows Ivan makes. If the battle will continue forever, print in the first line "Draw".</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>R</i></span> (<span class="tex-span">0 ≤ <i>h</i>, <i>t</i>, <i>R</i> ≤ 200</span>, <span class="tex-span">0 &lt; <i>h</i> + <i>t</i> ≤ <i>R</i></span>) which represent the initial numbers of Gorynych’s heads and tails and the largest total number of heads and tails with which Gorynych the Dragon does not yet attack. The next line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200</span>). The next <span class="tex-span"><i>n</i></span> contain pairs of non-negative numbers "<span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>" which represent the number of heads and the number of tails correspondingly, that will grow if Gorynych has <span class="tex-span"><i>i</i></span> heads (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) cut. The next line contains an integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200</span>) and then — the description of Gorynych’s behavior when his tails are cut off in the format identical to the one described above. All the numbers in the input file do not exceed <span class="tex-span">200</span>. </p>

## Output

<p>Print "Ivan" (without quotes) in the first line if Ivan wins, or "Zmey" (that means a dragon in Russian) if Gorynych the Dragon wins. In the second line print a single integer which represents the number of blows Ivan makes. If the battle will continue forever, print in the first line "Draw".</p>





```input1
2 2 4
2
1 0
0 1
3
0 1
0 1
0 0

```




```input2
2 2 4
1
0 1
1
1 0

```




```input3
2 2 5
1
1 1
1
3 0

```




```output1
Ivan
2

```




```output2
Draw

```




```output3
Zmey
2

```


