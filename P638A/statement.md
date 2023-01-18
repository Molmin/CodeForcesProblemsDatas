## Description

<div><p>The main street of Berland is a straight line with <span class="tex-span"><i>n</i></span> houses built along it (<span class="tex-span"><i>n</i></span> is an even number). The houses are located at both sides of the street. The houses with odd numbers are at one side of the street and are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span> in the order from the beginning of the street to the end (in the picture: from left to right). The houses with even numbers are at the other side of the street and are numbered from <span class="tex-span">2</span> to <span class="tex-span"><i>n</i></span> in the order from the end of the street to its beginning (in the picture: from right to left). The corresponding houses with even and odd numbers are strictly opposite each other, that is, house <span class="tex-span">1</span> is opposite house <span class="tex-span"><i>n</i></span>, house <span class="tex-span">3</span> is opposite house <span class="tex-span"><i>n</i> - 2</span>, house <span class="tex-span">5</span> is opposite house <span class="tex-span"><i>n</i> - 4</span> and so on.</p><center> <img class="tex-graphics" src="file://GalgVt4A.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Vasya needs to get to house number <span class="tex-span"><i>a</i></span> as quickly as possible. He starts driving from the beginning of the street and drives his car to house <span class="tex-span"><i>a</i></span>. To get from the beginning of the street to houses number <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>, he spends exactly <span class="tex-span">1</span> second. He also spends exactly one second to drive the distance between two neighbouring houses. Vasya can park at any side of the road, so the distance between the beginning of the street at the houses that stand opposite one another should be considered the same.</p><p>Your task is: find the minimum time Vasya needs to reach house <span class="tex-span"><i>a</i></span>.</p></div><div class="input-specification"><p>The first line of the input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of houses on the street and the number of the house that Vasya needs to reach, correspondingly. It is guaranteed that number <span class="tex-span"><i>n</i></span> is even.</p></div><div class="output-specification"><p>Print a single integer — the minimum time Vasya needs to get from the beginning of the street to house <span class="tex-span"><i>a</i></span>.</p></div>

## Input

<p>The first line of the input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of houses on the street and the number of the house that Vasya needs to reach, correspondingly. It is guaranteed that number <span class="tex-span"><i>n</i></span> is even.</p>

## Output

<p>Print a single integer — the minimum time Vasya needs to get from the beginning of the street to house <span class="tex-span"><i>a</i></span>.</p>





```input1
4 2

```




```input2
8 5

```




```output1
2

```




```output2
3

```



## Note

<p>In the first sample there are only four houses on the street, two houses at each side. House <span class="tex-span">2</span> will be the last at Vasya's right.</p><p>The second sample corresponds to picture with <span class="tex-span"><i>n</i> = 8</span>. House <span class="tex-span">5</span> is the one before last at Vasya's left.</p>
