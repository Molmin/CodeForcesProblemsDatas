## Description

<div><p>Polar bears like <span class="tex-font-style-it">unique arrays</span> — that is, arrays without repeated elements.</p><p> You have got a unique array <span class="tex-span"><i>s</i></span> with length <span class="tex-span"><i>n</i></span> containing non-negative integers. Since you are good friends with Alice and Bob, you decide to split the array in two. Precisely, you need to construct two arrays <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> that are also of length <span class="tex-span"><i>n</i></span>, with the following conditions for all <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>i</i> ≤ <i>n</i>)</span>:</p><ul> <li> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> are non-negative integers; </li><li> <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> = <i>a</i><sub class="lower-index"><i>i</i></sub> + <i>b</i><sub class="lower-index"><i>i</i></sub></span> . </li></ul><p>Ideally, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> should also be unique arrays. However, life in the Arctic is hard and this is not always possible. Fortunately, Alice and Bob are still happy if their arrays are <span class="tex-font-style-it">almost unique</span>. We define an array of length <span class="tex-span"><i>n</i></span> to be almost unique, if and only if it can be turned into a unique array by removing no more than <img align="middle" class="tex-formula" src="file://SpqQn6lX.png" style="max-width: 100.0%;max-height: 100.0%;"> entries.</p><p>For example, the array <span class="tex-span">[1, 2, 1, 3, 2]</span> is almost unique because after removing the first two entries, it becomes <span class="tex-span">[1, 3, 2]</span>. The array <span class="tex-span">[1, 2, 1, 3, 1, 2]</span> is not almost unique because we need to remove at least <span class="tex-span">3</span> entries to turn it into a unique array.</p><p>So, your task is to split the given unique array <span class="tex-span"><i>s</i></span> into two almost unique arrays <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ... <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>If it is possible to make Alice and Bob happy (if you can split the given array), print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line. In the second line, print the array <span class="tex-span"><i>a</i></span>. In the third line, print the array <span class="tex-span"><i>b</i></span>. There may be more than one solution. Any of them will be accepted.</p><p>If it is impossible to split <span class="tex-span"><i>s</i></span> into almost unique arrays <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, print "<span class="tex-font-style-tt">NO</span>" (without quotes) in the first line.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p><p>The second line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ... <i>s</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>If it is possible to make Alice and Bob happy (if you can split the given array), print "<span class="tex-font-style-tt">YES</span>" (without quotes) in the first line. In the second line, print the array <span class="tex-span"><i>a</i></span>. In the third line, print the array <span class="tex-span"><i>b</i></span>. There may be more than one solution. Any of them will be accepted.</p><p>If it is impossible to split <span class="tex-span"><i>s</i></span> into almost unique arrays <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, print "<span class="tex-font-style-tt">NO</span>" (without quotes) in the first line.</p>





```input1
6
12 5 8 3 11 9

```




```output1
YES
6 2 6 0 2 4
6 3 2 3 9 5
```



## Note

<p>In the sample, we can remove the first two entries from <span class="tex-span"><i>a</i></span> and the second entry from <span class="tex-span"><i>b</i></span> to make them both unique.</p>
