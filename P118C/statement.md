## Description

<div><p>A car number in Berland consists of exactly <span class="tex-span"><i>n</i></span> digits. A number is called beautiful if it has at least <span class="tex-span"><i>k</i></span> equal digits. Vasya wants to change the digits in his car's number so that the number became beautiful. To replace one of <span class="tex-span"><i>n</i></span> digits Vasya has to pay the sum of money, equal to the absolute difference between the old digit and the new one.</p><p>Help Vasya: find the minimum sum of money he should pay to make the number of his car beautiful. You should also find the resulting beautiful number. If there are several such numbers, then print the lexicographically minimum one.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>, 2 ≤ <i>k</i> ≤ <i>n</i></span>) which represent how many digits the number has and how many equal digits a beautiful number should have. The second line consists of <span class="tex-span"><i>n</i></span> digits. It describes the old number of Vasya's car. It is guaranteed that the number contains no spaces and only contains digits.</p></div><div class="output-specification"><p>On the first line print the minimum sum of money Vasya needs to change the number. On the second line print the car's new number. If there are several solutions, print the lexicographically minimum one.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>, 2 ≤ <i>k</i> ≤ <i>n</i></span>) which represent how many digits the number has and how many equal digits a beautiful number should have. The second line consists of <span class="tex-span"><i>n</i></span> digits. It describes the old number of Vasya's car. It is guaranteed that the number contains no spaces and only contains digits.</p>

## Output

<p>On the first line print the minimum sum of money Vasya needs to change the number. On the second line print the car's new number. If there are several solutions, print the lexicographically minimum one.</p>





```input1
6 5
898196

```




```input2
3 2
533

```




```input3
10 6
0001112223

```




```output1
4
888188

```




```output2
0
533

```




```output3
3
0000002223

```



## Note

<p>In the first sample replacing the second digit with an "<span class="tex-font-style-tt">8</span>" costs <span class="tex-span">|9 - 8| = 1</span>. Replacing the fifth digit with an "<span class="tex-font-style-tt">8</span>" costs the same. Replacing the sixth digit costs <span class="tex-span">|6 - 8| = 2</span>. As a result, Vasya will pay <span class="tex-span">1 + 1 + 2 = 4</span> for a beautiful number "<span class="tex-font-style-tt">888188</span>".</p><p>The lexicographical comparison of strings is performed by the &lt; operator in modern programming languages. The string <span class="tex-span"><i>x</i></span> is lexicographically smaller than the string <span class="tex-span"><i>y</i></span>, if there exists such <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>), that <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &lt; <i>y</i><sub class="lower-index"><i>i</i></sub></span>, and for any <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> &lt; <i>i</i></span>) <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub> = <i>y</i><sub class="lower-index"><i>j</i></sub></span>. The strings compared in this problem will always have the length <span class="tex-span"><i>n</i></span>.</p>
