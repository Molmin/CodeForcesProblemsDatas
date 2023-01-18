## Description

<div><p>Vasya and Kolya play a game with a string, using the following rules. Initially, Kolya creates a string <span class="tex-span"><i>s</i></span>, consisting of small English letters, and uniformly at random chooses an integer <span class="tex-span"><i>k</i></span> from a segment <span class="tex-span">[0, <i>len</i>(<i>s</i>) - 1]</span>. He tells Vasya this string <span class="tex-span"><i>s</i></span>, and then shifts it <span class="tex-span"><i>k</i></span> letters to the left, i.&nbsp;e. creates a new string <span class="tex-span"><i>t</i> = <i>s</i><sub class="lower-index"><i>k</i> + 1</sub><i>s</i><sub class="lower-index"><i>k</i> + 2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub><i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>k</i></sub></span>. Vasya does not know the integer <span class="tex-span"><i>k</i></span> nor the string <span class="tex-span"><i>t</i></span>, but he wants to guess the integer <span class="tex-span"><i>k</i></span>. To do this, he asks Kolya to tell him the first letter of the new string, and then, after he sees it, open one more letter on some position, which Vasya can choose.</p><p>Vasya understands, that he can't guarantee that he will win, but he wants to know the probability of winning, if he plays optimally. He wants you to compute this probability. </p><p>Note that Vasya wants to know the value of <span class="tex-span"><i>k</i></span> uniquely, it means, that if there are at least two cyclic shifts of <span class="tex-span"><i>s</i></span> that fit the information Vasya knowns, Vasya loses. Of course, at any moment of the game Vasya wants to maximize the probability of his win.</p></div><div class="input-specification"><p>The only string contains the string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>l</i></span> <span class="tex-span">(3 ≤ <i>l</i> ≤ 5000)</span>, consisting of small English letters only.</p></div><div class="output-specification"><p>Print the only number&nbsp;— the answer for the problem. You answer is considered correct, if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://fUWHVpPz.png" style="max-width: 100.0%;max-height: 100.0%;"></p></div>

## Input

<p>The only string contains the string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>l</i></span> <span class="tex-span">(3 ≤ <i>l</i> ≤ 5000)</span>, consisting of small English letters only.</p>

## Output

<p>Print the only number&nbsp;— the answer for the problem. You answer is considered correct, if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Formally, let your answer be <span class="tex-span"><i>a</i></span>, and the jury's answer be <span class="tex-span"><i>b</i></span>. Your answer is considered correct if <img align="middle" class="tex-formula" src="file://fUWHVpPz.png" style="max-width: 100.0%;max-height: 100.0%;"></p>





```input1
technocup

```




```input2
tictictactac

```




```input3
bbaabaabbb

```




```output1
1.000000000000000

```




```output2
0.333333333333333

```




```output3
0.100000000000000

```



## Note

<p>In the first example Vasya can always open the second letter after opening the first letter, and the cyclic shift is always determined uniquely.</p><p>In the second example if the first opened letter of <span class="tex-span"><i>t</i></span> is "<span class="tex-font-style-tt">t</span>" or "<span class="tex-font-style-tt">c</span>", then Vasya can't guess the shift by opening only one other letter. On the other hand, if the first letter is "<span class="tex-font-style-tt">i</span>" or "<span class="tex-font-style-tt">a</span>", then he can open the fourth letter and determine the shift uniquely.</p>
