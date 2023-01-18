## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>Natasha is going to fly to Mars. Finally, Natasha sat in the rocket. She flies, flies... but gets bored. She wishes to arrive to Mars already! So she decides to find something to occupy herself. She couldn't think of anything better to do than to calculate the distance to the red planet.</p><p>Let's define $x$ as the distance to Mars. Unfortunately, Natasha does not know $x$. But it is known that $1 \le x \le m$, where Natasha knows the number $m$. Besides, $x$ and $m$ are positive integers.</p><p>Natasha can ask the rocket questions. Every question is an integer $y$ ($1 \le y \le m$). The correct answer to the question is $-1$, if $x&lt;y$, $0$, if $x=y$, and $1$, if $x&gt;y$. But the rocket is broken&nbsp;— it does not always answer correctly. Precisely: let the correct answer to the current question be equal to $t$, then, if the rocket answers this question correctly, then it will answer $t$, otherwise it will answer $-t$.</p><p>In addition, the rocket has a sequence $p$ of length $n$. Each element of the sequence is either $0$ or $1$. The rocket processes this sequence in the cyclic order, that is $1$-st element, $2$-nd, $3$-rd, $\ldots$, $(n-1)$-th, $n$-th, $1$-st, $2$-nd, $3$-rd, $\ldots$, $(n-1)$-th, $n$-th, $\ldots$. If the current element is $1$, the rocket answers correctly, if $0$&nbsp;— lies. Natasha doesn't know the sequence $p$, but she knows its length&nbsp;— $n$.</p><p>You can ask the rocket no more than $60$ questions.</p><p>Help Natasha find the distance to Mars. Assume, that the distance to Mars does not change while Natasha is asking questions.</p><p>Your solution will not be accepted, if it does not receive an answer $0$ from the rocket (even if the distance to Mars is uniquely determined by the already received rocket's answers).</p></div><div class="input-specification"><p>The first line contains two integers $m$ and $n$ ($1 \le m \le 10^9$, $1 \le n \le 30$)&nbsp;— the maximum distance to Mars and the number of elements in the sequence $p$.</p></div><div><h2>Interaction</h2><p>You can ask the rocket no more than $60$ questions.</p><p>To ask a question, print a number $y$ ($1\le y\le m$) and an end-of-line character, then do the operation <span class="tex-font-style-tt">flush</span> and read the answer to the question.</p><p>If the program reads $0$, then the distance is correct and you must immediately terminate the program (for example, by calling <span class="tex-font-style-tt">exit(0)</span>). If you ignore this, you can get any verdict, since your program will continue to read from the closed input stream.</p><p>If at some point your program reads $-2$ as an answer, it must immediately end (for example, by calling <span class="tex-font-style-tt">exit(0)</span>). You will receive the "Wrong answer" verdict, and this will mean that the request is incorrect or the number of requests exceeds $60$. If you ignore this, you can get any verdict, since your program will continue to read from the closed input stream.</p><p>If your program's request is not a valid integer between $-2^{31}$ and $2^{31}-1$ (inclusive) without leading zeros, then you can get any verdict.</p><p>You can get "Idleness limit exceeded" if you don't print anything or if you forget to flush the output.</p><p>To flush the output buffer you can use (after printing a query and end-of-line):</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> See the documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacking</span></p><p>Use the following format for hacking:</p><p>In the first line, print $3$ integers $m,n,x$ ($1\le x\le m\le 10^9$, $1\le n\le 30$)&nbsp;— the maximum distance to Mars, the number of elements in the sequence $p$ and the current distance to Mars.</p><p>In the second line, enter $n$ numbers, each of which is equal to $0$ or $1$&nbsp;— sequence $p$.</p><p>The hacked solution will not have access to the number $x$ and sequence $p$.</p></div>

## Input

<p>The first line contains two integers $m$ and $n$ ($1 \le m \le 10^9$, $1 \le n \le 30$)&nbsp;— the maximum distance to Mars and the number of elements in the sequence $p$.</p>





```input1
5 2
1
-1
-1
1
0

```




```output1
1
2
4
5
3

```



## Note

<p>In the example, hacking would look like this:</p><p><span class="tex-font-style-tt">5 2 3</span></p><p><span class="tex-font-style-tt">1 0</span></p><p>This means that the current distance to Mars is equal to $3$, Natasha knows that it does not exceed $5$, and the rocket answers in order: correctly, incorrectly, correctly, incorrectly ...</p><p>Really:</p><p>on the first query ($1$) the correct answer is $1$, the rocket answered correctly: $1$;</p><p>on the second query ($2$) the correct answer is $1$, the rocket answered incorrectly: $-1$;</p><p>on the third query ($4$) the correct answer is $-1$, the rocket answered correctly: $-1$;</p><p>on the fourth query ($5$) the correct answer is $-1$, the rocket answered incorrectly: $1$;</p><p>on the fifth query ($3$) the correct and incorrect answer is $0$.</p>
