## Description

<div><p>A top-secret military base under the command of Colonel Zuev is expecting an inspection from the Ministry of Defence. According to the charter, each top-secret military base must include a top-secret troop that should... well, we cannot tell you exactly what it should do, it is a top secret troop at the end. The problem is that Zuev's base is missing this top-secret troop for some reasons.</p><p>The colonel decided to deal with the problem immediately and ordered to line up in a single line all <span class="tex-span"><i>n</i></span> soldiers of the base entrusted to him. Zuev knows that the <span class="tex-font-style-it">loquacity</span> of the <span class="tex-span"><i>i</i></span>-th soldier from the left is equal to <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span>. Zuev wants to form the top-secret troop using <span class="tex-span"><i>k</i></span> leftmost soldiers in the line, thus he wants their total loquacity to be as small as possible (as the troop should remain top-secret). To achieve this, he is going to choose a pair of <span class="tex-font-style-bf">consecutive</span> soldiers and swap them. He intends to do so no more than <span class="tex-span"><i>s</i></span> times. Note that any soldier can be a participant of such swaps for any number of times. The problem turned out to be unusual, and colonel Zuev asked you to help.</p><p>Determine, what is the minimum total loquacity of the first <span class="tex-span"><i>k</i></span> soldiers in the line, that can be achieved by performing no more than <span class="tex-span"><i>s</i></span> swaps of two consecutive soldiers.</p></div><div class="input-specification"><p>The first line of the input contains three positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 150</span>, <span class="tex-span">1 ≤ <i>s</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of soldiers in the line, the size of the top-secret troop to be formed and the maximum possible number of swap operations of the consecutive pair of soldiers, respectively.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integer <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the values of loquacity of soldiers in order they follow in line from left to right.</p></div><div class="output-specification"><p>Print a single integer — the minimum possible total loquacity of the top-secret troop.</p></div>

## Input

<p>The first line of the input contains three positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 150</span>, <span class="tex-span">1 ≤ <i>s</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of soldiers in the line, the size of the top-secret troop to be formed and the maximum possible number of swap operations of the consecutive pair of soldiers, respectively.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integer <span class="tex-span"><i>q</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>q</i><sub class="lower-index"><i>i</i></sub> ≤ 1 000 000</span>)&nbsp;— the values of loquacity of soldiers in order they follow in line from left to right.</p>

## Output

<p>Print a single integer — the minimum possible total loquacity of the top-secret troop.</p>





```input1
3 2 2
2 4 1

```




```input2
5 4 2
10 1 6 2 5

```




```input3
5 2 3
3 1 4 2 5

```




```output1
3

```




```output2
18

```




```output3
3

```



## Note

<p>In the first sample Colonel has to swap second and third soldiers, he doesn't really need the remaining swap. The resulting soldiers order is: (<span class="tex-span">2</span>, <span class="tex-span">1</span>, <span class="tex-span">4</span>). Minimum possible summary loquacity of the secret troop is <span class="tex-span">3</span>. In the second sample Colonel will perform swaps in the following order:</p><ol> <li> (10, 1, <span class="tex-font-style-bf">6</span> — <span class="tex-font-style-bf">2</span>, 5) </li><li> (10, 1, 2, <span class="tex-font-style-bf">6</span> — <span class="tex-font-style-bf">5</span>) </li></ol><p>The resulting soldiers order is (10, 1, 2, 5, 6). </p><p>Minimum possible summary loquacity is equal to <span class="tex-span">18</span>.</p>
