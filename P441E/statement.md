## Description

<div><p>Valera is a coder. Recently he wrote a funny program. The pseudo code for this program is given below:</p><pre class="verbatim"><br>//input: integers x, k, p<br>a = x;<br>for(step = 1; step &lt;= k; step = step + 1){<br>    rnd = [random integer from 1 to 100];<br>    if(rnd &lt;= p)<br>        a = a * 2;<br>    else<br>        a = a + 1;<br>}<br><br>s = 0;<br><br>while(remainder after dividing a by 2 equals 0){<br>    a = a / 2;<br>    s = s + 1;<br>}<br><br></pre><p>Now Valera wonders: given the values <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>p</i></span>, what is the expected value of the resulting number <span class="tex-span"><i>s</i></span>?</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>x</i>, <i>k</i>, <i>p</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>k</i> ≤ 200;&nbsp;0 ≤ <i>p</i> ≤ 100</span>).</p></div><div class="output-specification"><p>Print the required expected value. Your answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>x</i>, <i>k</i>, <i>p</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ 10<sup class="upper-index">9</sup>;&nbsp;1 ≤ <i>k</i> ≤ 200;&nbsp;0 ≤ <i>p</i> ≤ 100</span>).</p>

## Output

<p>Print the required expected value. Your answer will be considered correct if the absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
1 1 50

```




```input2
5 3 0

```




```input3
5 3 25

```




```output1
1.0000000000000

```




```output2
3.0000000000000

```




```output3
1.9218750000000

```



## Note

<p>If the concept of expected value is new to you, you can read about it by the link: </p><p>http://en.wikipedia.org/wiki/Expected_value</p>
