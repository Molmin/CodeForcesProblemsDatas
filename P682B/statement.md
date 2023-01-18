## Description

<div><p>Someone gave Alyona an array containing <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. In one operation, Alyona can choose any element of the array and decrease it, i.e. replace with any positive integer that is smaller than the current one. Alyona can repeat this operation as many times as she wants. In particular, she may not apply any operation to the array at all.</p><p>Formally, after applying some operations Alyona will get an array of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> such that <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub></span> for every <span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>. Your task is to determine the maximum possible value of mex of this array.</p><p><span class="tex-font-style-it">Mex</span> of an array in this problem is the <span class="tex-font-style-bf">minimum positive</span> integer that doesn't appear in this array. For example, mex of the array containing <span class="tex-span">1</span>, <span class="tex-span">3</span> and <span class="tex-span">4</span> is equal to <span class="tex-span">2</span>, while mex of the array containing <span class="tex-span">2</span>, <span class="tex-span">3</span> and <span class="tex-span">2</span> is equal to <span class="tex-span">1</span>.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of elements in the Alyona's array.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of the array.</p></div><div class="output-specification"><p>Print one positive integer&nbsp;— the maximum possible value of mex of the array after Alyona applies some (possibly none) operations.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of elements in the Alyona's array.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the elements of the array.</p>

## Output

<p>Print one positive integer&nbsp;— the maximum possible value of mex of the array after Alyona applies some (possibly none) operations.</p>





```input1
5
1 3 3 3 6

```




```input2
2
2 1

```




```output1
5

```




```output2
3

```



## Note

<p>In the first sample case if one will decrease the second element value to <span class="tex-span">2</span> and the fifth element value to <span class="tex-span">4</span> then the <span class="tex-font-style-it">mex</span> value of resulting array <span class="tex-span">1</span> <span class="tex-span">2</span> <span class="tex-span">3</span> <span class="tex-span">3</span> <span class="tex-span">4</span> will be equal to <span class="tex-span">5</span>.</p><p>To reach the answer to the second sample case one must not decrease any of the array elements.</p>
