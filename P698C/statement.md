## Description

<div><p>While creating high loaded systems one should pay a special attention to caching. This problem will be about one of the most popular caching algorithms called LRU (Least Recently Used).</p><p>Suppose the cache may store no more than <span class="tex-span"><i>k</i></span> objects. At the beginning of the workflow the cache is empty. When some object is queried we check if it is present in the cache and move it here if it's not. If there are more than <span class="tex-span"><i>k</i></span> objects in the cache after this, the least recently used one should be removed. In other words, we remove the object that has the smallest time of the last query.</p><p>Consider there are <span class="tex-span"><i>n</i></span> videos being stored on the server, all of the same size. Cache can store no more than <span class="tex-span"><i>k</i></span> videos and caching algorithm described above is applied. We know that any time a user enters the server he pick the video <span class="tex-span"><i>i</i></span> with probability <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. The choice of the video is independent to any events before.</p><p>The goal of this problem is to count for each of the videos the probability it will be present in the cache after <span class="tex-span">10<sup class="upper-index">100</sup></span> queries.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 20</span>)&nbsp;— the number of videos and the size of the cache respectively. Next line contains <span class="tex-span"><i>n</i></span> real numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), each of them is given with no more than two digits after decimal point.</p><p>It's guaranteed that the sum of all <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is equal to <span class="tex-span">1</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> real numbers, the <span class="tex-span"><i>i</i></span>-th of them should be equal to the probability that the <span class="tex-span"><i>i</i></span>-th video will be present in the cache after <span class="tex-span">10<sup class="upper-index">100</sup></span> queries. You answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://ciYCfVAa.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 20</span>)&nbsp;— the number of videos and the size of the cache respectively. Next line contains <span class="tex-span"><i>n</i></span> real numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1</span>), each of them is given with no more than two digits after decimal point.</p><p>It's guaranteed that the sum of all <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> is equal to <span class="tex-span">1</span>.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> real numbers, the <span class="tex-span"><i>i</i></span>-th of them should be equal to the probability that the <span class="tex-span"><i>i</i></span>-th video will be present in the cache after <span class="tex-span">10<sup class="upper-index">100</sup></span> queries. You answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://ciYCfVAa.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3 1
0.3 0.2 0.5

```




```input2
2 1
0.0 1.0

```




```input3
3 2
0.3 0.2 0.5

```




```input4
3 3
0.2 0.3 0.5

```




```output1
0.3 0.2 0.5
```




```output2
0.0 1.0
```




```output3
0.675 0.4857142857142857 0.8392857142857143
```




```output4
1.0 1.0 1.0
```


