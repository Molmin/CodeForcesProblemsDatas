## Description

<div><p>The year 2015 is almost over.</p><p>Limak is a little polar bear. He has recently learnt about the binary system. He noticed that the passing year has exactly one zero in its representation in the binary system&nbsp;— <span class="tex-span">2015<sub class="lower-index">10</sub> = 11111011111<sub class="lower-index">2</sub></span>. Note that he doesn't care about the number of zeros in the decimal representation.</p><p>Limak chose some interval of years. He is going to count all years from this interval that have exactly one zero in the binary representation. Can you do it faster?</p><p>Assume that all positive integers are always written without leading zeros.</p></div><div class="input-specification"><p>The only line of the input contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the first year and the last year in Limak's interval respectively.</p></div><div class="output-specification"><p>Print one integer&nbsp;– the number of years Limak will count in his chosen interval.</p></div>

## Input

<p>The only line of the input contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the first year and the last year in Limak's interval respectively.</p>

## Output

<p>Print one integer&nbsp;– the number of years Limak will count in his chosen interval.</p>





```input1
5 10

```




```input2
2015 2015

```




```input3
100 105

```




```input4
72057594000000000 72057595000000000

```




```output1
2

```




```output2
1

```




```output3
0

```




```output4
26

```



## Note

<p>In the first sample Limak's interval contains numbers <span class="tex-span">5<sub class="lower-index">10</sub> = 101<sub class="lower-index">2</sub></span>, <span class="tex-span">6<sub class="lower-index">10</sub> = 110<sub class="lower-index">2</sub></span>, <span class="tex-span">7<sub class="lower-index">10</sub> = 111<sub class="lower-index">2</sub></span>, <span class="tex-span">8<sub class="lower-index">10</sub> = 1000<sub class="lower-index">2</sub></span>, <span class="tex-span">9<sub class="lower-index">10</sub> = 1001<sub class="lower-index">2</sub></span> and <span class="tex-span">10<sub class="lower-index">10</sub> = 1010<sub class="lower-index">2</sub></span>. Two of them (<span class="tex-span">101<sub class="lower-index">2</sub></span> and <span class="tex-span">110<sub class="lower-index">2</sub></span>) have the described property.</p>
