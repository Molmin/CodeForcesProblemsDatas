## Description

<div><p>Winnie-the-Pooh likes honey very much! That is why he decided to visit his friends. Winnie has got three best friends: Rabbit, Owl and Eeyore, each of them lives in his own house. There are winding paths between each pair of houses. The length of a path between Rabbit's and Owl's houses is <span class="tex-span"><i>a</i></span> meters, between Rabbit's and Eeyore's house is <span class="tex-span"><i>b</i></span> meters, between Owl's and Eeyore's house is <span class="tex-span"><i>c</i></span> meters.</p><p>For enjoying his life and singing merry songs Winnie-the-Pooh should have a meal <span class="tex-span"><i>n</i></span> times a day. Now he is in the Rabbit's house and has a meal for the first time. Each time when in the friend's house where Winnie is now the supply of honey is about to end, Winnie leaves that house. If Winnie has not had a meal the required amount of times, he comes out from the house and goes to someone else of his two friends. For this he chooses one of two adjacent paths, arrives to the house on the other end and visits his friend. You may assume that when Winnie is eating in one of his friend's house, the supply of honey in other friend's houses recover (most probably, they go to the supply store).</p><p>Winnie-the-Pooh does not like physical activity. He wants to have a meal <span class="tex-span"><i>n</i></span> times, traveling minimum possible distance. Help him to find this distance.</p></div><div class="input-specification"><p>First line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— number of visits.</p><p>Second line contains an integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 100</span>)&nbsp;— distance between Rabbit's and Owl's houses.</p><p>Third line contains an integer <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ 100</span>)&nbsp;— distance between Rabbit's and Eeyore's houses.</p><p>Fourth line contains an integer <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>c</i> ≤ 100</span>)&nbsp;— distance between Owl's and Eeyore's houses.</p></div><div class="output-specification"><p>Output one number&nbsp;— minimum distance in meters Winnie must go through to have a meal <span class="tex-span"><i>n</i></span> times.</p></div>

## Input

<p>First line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>)&nbsp;— number of visits.</p><p>Second line contains an integer <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 100</span>)&nbsp;— distance between Rabbit's and Owl's houses.</p><p>Third line contains an integer <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ 100</span>)&nbsp;— distance between Rabbit's and Eeyore's houses.</p><p>Fourth line contains an integer <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>c</i> ≤ 100</span>)&nbsp;— distance between Owl's and Eeyore's houses.</p>

## Output

<p>Output one number&nbsp;— minimum distance in meters Winnie must go through to have a meal <span class="tex-span"><i>n</i></span> times.</p>





```input1
3
2
3
1

```




```input2
1
2
3
5

```




```output1
3

```




```output2
0

```



## Note

<p>In the first test case the optimal path for Winnie is the following: first have a meal in Rabbit's house, then in Owl's house, then in Eeyore's house. Thus he will pass the distance <span class="tex-span">2 + 1 = 3</span>.</p><p>In the second test case Winnie has a meal in Rabbit's house and that is for him. So he doesn't have to walk anywhere at all.</p>
