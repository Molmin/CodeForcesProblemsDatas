## Description

<div><p>Developer Petr thinks that he invented a perpetual motion machine. Namely, he has a lot of <span class="tex-font-style-it">elements</span>, which work in the following way.</p><p>Each element has one controller that can be set to any non-negative real value. If a controller is set on some value <span class="tex-span"><i>x</i></span>, then the controller consumes <span class="tex-span"><i>x</i><sup class="upper-index">2</sup></span> energy units per second. At the same time, any two elements connected by a wire produce <span class="tex-span"><i>y</i>·<i>z</i></span> energy units per second, where <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> are the values set on their controllers.</p><p>Petr has only a limited number of wires, so he has already built some scheme of elements and wires, and is now interested if it's possible to set the controllers in such a way that the system produces <span class="tex-font-style-bf">at least as much</span> power as it consumes, and at least one controller is set on the value different from <span class="tex-span">0</span>. Help him check this, and if it's possible, find the required <span class="tex-font-style-bf">integer</span> values that should be set.</p><p>It is guaranteed that if there exist controllers' settings satisfying the above conditions, then there exist required integer values not greater than <span class="tex-span">10<sup class="upper-index">6</sup></span>.</p></div><div class="input-specification"><p>There are several (at least one) test cases in the input. The first line contains single integer&nbsp;— the number of test cases.</p><p>There is an empty line before each test case. The first line of test case contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of elements in the scheme and the number of wires.</p><p>After that, <span class="tex-span"><i>m</i></span> lines follow, each of them contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>)&nbsp;— two elements connected by a wire. No element is connected with itself, no two elements are connected by more than one wire.</p><p>It is guaranteed that the sum of <span class="tex-span"><i>n</i></span> and the sum of <span class="tex-span"><i>m</i></span> over all test cases do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p><span class="tex-font-style-bf">For hacks</span> you can only use tests with one test case.</p></div><div class="output-specification"><p>Print answer for each test case.</p><p>For each test case print "<span class="tex-font-style-tt">YES</span>" if it's possible to set the controllers in such a way that the consumed power is not greater than the power produced, and the required values on the next line. The settings should be integers from <span class="tex-span">0</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span>, inclusive, and at least one value should be different from <span class="tex-span">0</span>. If there are multiple answers, print any of them.</p><p>If it's not possible to set the controllers in the required way, print one line "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>There are several (at least one) test cases in the input. The first line contains single integer&nbsp;— the number of test cases.</p><p>There is an empty line before each test case. The first line of test case contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of elements in the scheme and the number of wires.</p><p>After that, <span class="tex-span"><i>m</i></span> lines follow, each of them contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>)&nbsp;— two elements connected by a wire. No element is connected with itself, no two elements are connected by more than one wire.</p><p>It is guaranteed that the sum of <span class="tex-span"><i>n</i></span> and the sum of <span class="tex-span"><i>m</i></span> over all test cases do not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p><p><span class="tex-font-style-bf">For hacks</span> you can only use tests with one test case.</p>

## Output

<p>Print answer for each test case.</p><p>For each test case print "<span class="tex-font-style-tt">YES</span>" if it's possible to set the controllers in such a way that the consumed power is not greater than the power produced, and the required values on the next line. The settings should be integers from <span class="tex-span">0</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span>, inclusive, and at least one value should be different from <span class="tex-span">0</span>. If there are multiple answers, print any of them.</p><p>If it's not possible to set the controllers in the required way, print one line "<span class="tex-font-style-tt">NO</span>".</p>





```input1
4
&nbsp;
4 4
1 2
2 3
3 4
4 2
&nbsp;
3 2
2 3
3 1
&nbsp;
4 6
1 2
3 4
4 2
1 4
1 3
3 2
&nbsp;
10 9
2 1
3 2
5 2
6 2
2 7
2 8
2 9
2 10
4 2

```




```output1
YES
1 2 2 1
NO
YES
1 1 1 1
YES
1 5 1 1 1 1 1 1 1 1

```



## Note

<p>In the first example it's possible to set the controllers in the required way, for example, in the following way: set <span class="tex-span">1</span> on the first element, set <span class="tex-span">2</span> on the second and on the third, set <span class="tex-span">1</span> on the fourth. The consumed power is then equal to <span class="tex-span">1<sup class="upper-index">2</sup> + 2<sup class="upper-index">2</sup> + 2<sup class="upper-index">2</sup> + 1<sup class="upper-index">2</sup> = 10</span> energy units per second, the produced power is equal to <span class="tex-span">1·2 + 2·2 + 2·1 + 2·1 = 10</span> energy units per second. Thus the answer is "<span class="tex-font-style-tt">YES</span>".</p><p>In the second test case it's not possible to set the controllers in the required way. For example, if we set all controllers to <span class="tex-span">0.5</span>, then the consumed powers equals <span class="tex-span">0.75</span> energy units per second, while produced power equals <span class="tex-span">0.5</span> energy units per second.</p>
