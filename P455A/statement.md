## Description

<div><p>Alex doesn't like boredom. That's why whenever he gets bored, he comes up with games. One long winter evening he came up with a game and decided to play it.</p><p>Given a sequence <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> integers. The player can make several steps. In a single step he can choose an element of the sequence (let's denote it <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span>) and delete it, at that all elements equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub> + 1</span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub> - 1</span> also must be deleted from the sequence. That step brings <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub></span> points to the player. </p><p>Alex is a perfectionist, so he decided to get as many points as possible. Help him.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) that shows how many numbers are in Alex's sequence. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Print a single integer — the maximum number of points that Alex can earn.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) that shows how many numbers are in Alex's sequence. </p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Print a single integer — the maximum number of points that Alex can earn.</p>





```input1
2
1 2

```




```input2
3
1 2 3

```




```input3
9
1 2 1 3 2 2 2 2 3

```




```output1
2

```




```output2
4

```




```output3
10

```



## Note

<p>Consider the third test example. At first step we need to choose any element equal to <span class="tex-span">2</span>. After that step our sequence looks like this <span class="tex-span">[2, 2, 2, 2]</span>. Then we do <span class="tex-span">4</span> steps, on each step we choose any element equals to <span class="tex-span">2</span>. In total we earn <span class="tex-span">10</span> points.</p>
