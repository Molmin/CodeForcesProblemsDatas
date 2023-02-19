## Description

<div><p>Comrade Dujikov is busy choosing artists for Timofey's birthday and is recieving calls from Taymyr from Ilia-alpinist.</p><p>Ilia-alpinist calls every <span class="tex-span"><i>n</i></span> minutes, i.e. in minutes <span class="tex-span"><i>n</i></span>, <span class="tex-span">2<i>n</i></span>, <span class="tex-span">3<i>n</i></span> and so on. Artists come to the comrade every <span class="tex-span"><i>m</i></span> minutes, i.e. in minutes <span class="tex-span"><i>m</i></span>, <span class="tex-span">2<i>m</i></span>, <span class="tex-span">3<i>m</i></span> and so on. The day is <span class="tex-span"><i>z</i></span> minutes long, i.e. the day consists of minutes <span class="tex-span">1, 2, ..., <i>z</i></span>. How many artists should be killed so that there are no artists in the room when Ilia calls? Consider that a call and a talk with an artist take exactly one minute.</p></div><div class="input-specification"><p>The only string contains three integers&nbsp;— <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>z</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>z</i> ≤ 10<sup class="upper-index">4</sup></span>).</p></div><div class="output-specification"><p>Print single integer&nbsp;— the minimum number of artists that should be killed so that there are no artists in the room when Ilia calls.</p></div>

## Input

<p>The only string contains three integers&nbsp;— <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>z</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>z</i> ≤ 10<sup class="upper-index">4</sup></span>).</p>

## Output

<p>Print single integer&nbsp;— the minimum number of artists that should be killed so that there are no artists in the room when Ilia calls.</p>





```input1
1 1 10

```




```input2
1 2 5

```




```input3
2 3 9

```




```output1
10

```




```output2
2

```




```output3
1

```



## Note

<p>Taymyr is a place in the north of Russia.</p><p>In the first test the artists come each minute, as well as the calls, so we need to kill all of them.</p><p>In the second test we need to kill artists which come on the second and the fourth minutes.</p><p>In the third test&nbsp;— only the artist which comes on the sixth minute. </p>
