## Description

<div><p>Bear Limak wants to become the largest of bears, or at least to become larger than his brother Bob.</p><p>Right now, Limak and Bob weigh <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> respectively. It's guaranteed that Limak's weight is smaller than or equal to his brother's weight.</p><p>Limak eats a lot and his weight is tripled after every year, while Bob's weight is doubled after every year.</p><p>After how many full years will Limak become strictly larger (strictly heavier) than Bob?</p></div><div class="input-specification"><p>The only line of the input contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ 10</span>)&nbsp;— the weight of Limak and the weight of Bob respectively.</p></div><div class="output-specification"><p>Print one integer, denoting the integer number of years after which Limak will become strictly larger than Bob.</p></div>

## Input

<p>The only line of the input contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>b</i> ≤ 10</span>)&nbsp;— the weight of Limak and the weight of Bob respectively.</p>

## Output

<p>Print one integer, denoting the integer number of years after which Limak will become strictly larger than Bob.</p>





```input1
4 7

```




```input2
4 9

```




```input3
1 1

```




```output1
2

```




```output2
3

```




```output3
1

```



## Note

<p>In the first sample, Limak weighs <span class="tex-span">4</span> and Bob weighs <span class="tex-span">7</span> initially. After one year their weights are <span class="tex-span">4·3 = 12</span> and <span class="tex-span">7·2 = 14</span> respectively (one weight is tripled while the other one is doubled). Limak isn't larger than Bob yet. After the second year weights are <span class="tex-span">36</span> and <span class="tex-span">28</span>, so the first weight is greater than the second one. Limak became larger than Bob after two years so you should print <span class="tex-span">2</span>.</p><p>In the second sample, Limak's and Bob's weights in next years are: <span class="tex-span">12</span> and <span class="tex-span">18</span>, then <span class="tex-span">36</span> and <span class="tex-span">36</span>, and finally <span class="tex-span">108</span> and <span class="tex-span">72</span> (after three years). The answer is <span class="tex-span">3</span>. Remember that Limak wants to be larger than Bob and he won't be satisfied with equal weights.</p><p>In the third sample, Limak becomes larger than Bob after the first year. Their weights will be <span class="tex-span">3</span> and <span class="tex-span">2</span> then.</p>
