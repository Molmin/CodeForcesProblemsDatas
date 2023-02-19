## Description

<div><p>You have $n$ stacks of blocks. The $i$-th stack contains $h_i$ blocks and it's height is the number of blocks in it. In one move you can take a block from the $i$-th stack (if there is at least one block) and put it to the $i + 1$-th stack. Can you make the sequence of heights strictly increasing?</p><p>Note that the number of stacks always remains $n$: stacks don't disappear when they have $0$ blocks.</p></div><div class="input-specification"><p>First line contains a single integer $t$ $(1 \leq t \leq 10^4)$ — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ $(1 \leq n \leq 100)$. The second line of each test case contains $n$ integers $h_i$ $(0 \leq h_i \leq 10^9)$ — starting heights of the stacks.</p><p>It's guaranteed that the sum of all $n$ does not exceed $10^4$.</p></div><div class="output-specification"><p>For each test case output <span class="tex-font-style-tt">YES</span> if you can make the sequence of heights strictly increasing and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You may print each letter in any case (for example, <span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">Yes</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">yEs</span> will all be recognized as positive answer).</p></div>

## Input

<p>First line contains a single integer $t$ $(1 \leq t \leq 10^4)$ — the number of test cases.</p><p>The first line of each test case contains a single integer $n$ $(1 \leq n \leq 100)$. The second line of each test case contains $n$ integers $h_i$ $(0 \leq h_i \leq 10^9)$ — starting heights of the stacks.</p><p>It's guaranteed that the sum of all $n$ does not exceed $10^4$.</p>

## Output

<p>For each test case output <span class="tex-font-style-tt">YES</span> if you can make the sequence of heights strictly increasing and <span class="tex-font-style-tt">NO</span> otherwise.</p><p>You may print each letter in any case (for example, <span class="tex-font-style-tt">YES</span>, <span class="tex-font-style-tt">Yes</span>, <span class="tex-font-style-tt">yes</span>, <span class="tex-font-style-tt">yEs</span> will all be recognized as positive answer).</p>





```input1
6
2
1 2
2
1 0
3
4 4 4
2
0 0
3
0 1 0
4
1000000000 1000000000 1000000000 1000000000
```




```output1
YES
YES
YES
NO
NO
YES
```



## Note

<p>In the first test case there is no need to make any moves, the sequence of heights is already increasing.</p><p>In the second test case we need to move one block from the first stack to the second. Then the heights become $0$ $1$.</p><p>In the third test case we could move one block from the first stack to the second and then from the second to the third, which would make the heights $3$ $4$ $5$.</p><p>In the fourth test case we can't make a move, but the sequence is not increasing, so the answer is <span class="tex-font-style-tt">NO</span>.</p><p>In the fifth test case we can only make one move (from the second to the third stack), which would make the heights $0$ $0$ $1$. Both $0$ $1$ $0$ and $0$ $0$ $1$ are not increasing sequences, so the answer is <span class="tex-font-style-tt">NO</span>.</p>
