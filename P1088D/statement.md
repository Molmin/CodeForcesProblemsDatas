## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem!</span></p><p>Ehab plays a game with Laggy. Ehab has 2 hidden integers $(a,b)$. Laggy can ask a pair of integers $(c,d)$ and Ehab will reply with:</p><ul> <li> 1 if $a \oplus c&gt;b \oplus d$. </li><li> 0 if $a \oplus c=b \oplus d$. </li><li> -1 if $a \oplus c&lt;b \oplus d$. </li></ul><p>Operation $a \oplus b$ is the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise-xor operation</a> of two numbers $a$ and $b$.</p><p>Laggy should guess $(a,b)$ with <span class="tex-font-style-bf">at most 62 questions</span>. You'll play this game. You're Laggy and the interactor is Ehab.</p><p><span class="tex-font-style-bf">It's guaranteed that $0 \le a,b&lt;2^{30}$.</span></p></div><div class="input-specification"><p>See the interaction section.</p></div><div class="output-specification"><p>To print the answer, print "! a b" (without quotes). <span class="tex-font-style-bf">Don't forget to flush the output after printing the answer</span>.</p></div><div><h2>Interaction</h2><p>To ask a question, print "? c d" (without quotes). Both $c$ and $d$ must be non-negative integers less than $2^{30}$. <span class="tex-font-style-bf">Don't forget to flush the output after printing any question</span>.</p><p>After each question, you should read the answer as mentioned in the legend. If the interactor replies with -2, that means you asked more than 62 queries and your program should terminate.</p><p>To flush the output, you can use:-</p><ul> <li> fflush(stdout) in C++. </li><li> System.out.flush() in Java. </li><li> stdout.flush() in Python. </li><li> flush(output) in Pascal. </li><li> See the documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacking:</span></p><p>To hack someone, print the 2 space-separated integers $a$ and $b$ $(0 \le a,b&lt;2^{30})$.</p></div>

## Input

<p>See the interaction section.</p>

## Output

<p>To print the answer, print "! a b" (without quotes). <span class="tex-font-style-bf">Don't forget to flush the output after printing the answer</span>.</p>





```input1
1
-1
0
```




```output1
? 2 1
? 1 2
? 2 0
! 3 1
```



## Note

<p>In the sample:</p><p>The hidden numbers are $a=3$ and $b=1$.</p><p>In the first query: $3 \oplus 2 = 1$ and $1 \oplus 1 = 0$, so the answer is 1.</p><p>In the second query: $3 \oplus 1 = 2$ and $1 \oplus 2 = 3$, so the answer is -1.</p><p>In the third query: $3 \oplus 2 = 1$ and $1 \oplus 0 = 1$, so the answer is 0.</p><p>Then, we printed the answer.</p>
