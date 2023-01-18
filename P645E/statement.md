## Description

<div><p>After getting kicked out of her reporting job for not knowing the alphabet, Bessie has decided to attend school at the Fillet and Eggs Eater Academy. She has been making good progress with her studies and now knows the first <span class="tex-span"><i>k</i></span> English letters.</p><p>Each morning, Bessie travels to school along a sidewalk consisting of <span class="tex-span"><i>m</i> + <i>n</i></span> tiles. In order to help Bessie review, Mr. Moozing has labeled each of the first <span class="tex-span"><i>m</i></span> sidewalk tiles with one of the first <span class="tex-span"><i>k</i></span> lowercase English letters, spelling out a string <span class="tex-span"><i>t</i></span>. Mr. Moozing, impressed by Bessie's extensive knowledge of farm animals, plans to let her finish labeling the last <span class="tex-span"><i>n</i></span> tiles of the sidewalk by herself.</p><p>Consider the resulting string <span class="tex-span"><i>s</i></span> (<span class="tex-span">|<i>s</i>| = <i>m</i> + <i>n</i></span>) consisting of letters labeled on tiles in order from home to school. For any sequence of indices <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> &lt; <i>p</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>p</i><sub class="lower-index"><i>q</i></sub></span> we can define subsequence of the string <span class="tex-span"><i>s</i></span> as string <span class="tex-span"><i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index">1</sub></sub><i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index">2</sub></sub>... <i>s</i><sub class="lower-index"><i>p</i><sub class="lower-index"><i>q</i></sub></sub></span>. Two subsequences are considered to be distinct if they differ as strings. Bessie wants to label the remaining part of the sidewalk such that the number of <span class="tex-font-style-bf">distinct subsequences</span> of tiles is maximum possible. However, since Bessie hasn't even finished learning the alphabet, she needs your help!</p><p>Note that empty subsequence also counts.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 1 000 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 26</span>).</p><p>The second line contains a string <span class="tex-span"><i>t</i></span> (<span class="tex-span">|<i>t</i>| = <i>m</i>, 1 ≤ <i>m</i> ≤ 1 000 000</span>) consisting of only first <span class="tex-span"><i>k</i></span> lowercase English letters.</p></div><div class="output-specification"><p>Determine the maximum number of distinct subsequences Bessie can form after labeling the last <span class="tex-span"><i>n</i></span> sidewalk tiles each with one of the first <span class="tex-span"><i>k</i></span> lowercase English letters. Since this number can be rather large, you should print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Please note, that you are not asked to maximize the remainder modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>! The goal is to maximize the initial value and then print the remainder.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 1 000 000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 26</span>).</p><p>The second line contains a string <span class="tex-span"><i>t</i></span> (<span class="tex-span">|<i>t</i>| = <i>m</i>, 1 ≤ <i>m</i> ≤ 1 000 000</span>) consisting of only first <span class="tex-span"><i>k</i></span> lowercase English letters.</p>

## Output

<p>Determine the maximum number of distinct subsequences Bessie can form after labeling the last <span class="tex-span"><i>n</i></span> sidewalk tiles each with one of the first <span class="tex-span"><i>k</i></span> lowercase English letters. Since this number can be rather large, you should print it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Please note, that you are not asked to maximize the remainder modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>! The goal is to maximize the initial value and then print the remainder.</p>





```input1
1 3
ac

```




```input2
0 2
aaba

```




```output1
8

```




```output2
10

```



## Note

<p>In the first sample, the optimal labeling gives <span class="tex-span">8</span> different subsequences: "" (the empty string), "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">ac</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">cb</span>", and "<span class="tex-font-style-tt">acb</span>".</p><center> <img class="tex-graphics" src="file://YcUgUjA7.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the second sample, the entire sidewalk is already labeled. The are <span class="tex-span">10</span> possible different subsequences: "" (the empty string), "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">ba</span>", "<span class="tex-font-style-tt">aaa</span>", "<span class="tex-font-style-tt">aab</span>", "<span class="tex-font-style-tt">aba</span>", and "<span class="tex-font-style-tt">aaba</span>". Note that some strings, including "<span class="tex-font-style-tt">aa</span>", can be obtained with multiple sequences of tiles, but are only counted once.</p>
