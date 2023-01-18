## Description

<div><p><span class="tex-font-style-it">This is the hard version of the problem. You can find the easy version in the Div. 2 contest. Both versions only differ in the number of times you can ask your friend to taste coffee.</span></p><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>You're considering moving to another city, where one of your friends already lives. There are $n$ cafés in this city, where $n$ is a power of two. The $i$-th café produces a single variety of coffee $a_i$. </p><p>As you're a coffee-lover, before deciding to move or not, <span class="tex-font-style-bf">you want to know the number $d$ of distinct varieties of coffees</span> produced in this city.</p><p>You don't know the values $a_1, \ldots, a_n$. Fortunately, your friend has a memory of size $k$, where $k$ is a power of two.</p><p>Once per day, you can ask him to taste a cup of coffee produced by the café $c$, and he will tell you if he tasted a similar coffee during the last $k$ days.</p><p>You can also ask him to take a medication that will reset his memory. He will forget all previous cups of coffee tasted. You can reset his memory at most $30\ 000$ times.</p><p>More formally, the memory of your friend is a queue $S$. Doing a query on café $c$ will: </p><ul> <li> Tell you if $a_c$ is in $S$; </li><li> Add $a_c$ at the back of $S$; </li><li> If $|S| &gt; k$, pop the front element of $S$. </li></ul><p>Doing a reset request will pop all elements out of $S$.</p><p>Your friend can taste at most $\dfrac{3n^2}{2k}$ cups of coffee in total. Find the diversity $d$ (number of distinct values in the array $a$).</p><p>Note that asking your friend to reset his memory <span class="tex-font-style-bf">does not count</span> towards the number of times you ask your friend to taste a cup of coffee.</p><p>In some test cases the behavior of the interactor <span class="tex-font-style-bf">is adaptive</span>. It means that the array $a$ may be <span class="tex-font-style-bf">not fixed</span> before the start of the interaction and may <span class="tex-font-style-bf">depend on your queries</span>. It is guaranteed that at any moment of the interaction, there is at least one array $a$ consistent with all the answers given so far.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 1024$, $k$ and $n$ are powers of two).</p><p>It is guaranteed that $\dfrac{3n^2}{2k} \le 15\ 000$.</p></div><div><h2>Interaction</h2><p>You begin the interaction by reading $n$ and $k$.</p><ul><li> To ask your friend to taste a cup of coffee produced by the café $c$, in a separate line output<p><span class="tex-font-style-tt">? $c$</span></p><p>Where $c$ must satisfy $1 \le c \le n$. Don't forget to flush, to get the answer.</p><p>In response, you will receive a single letter <span class="tex-font-style-tt">Y</span> (yes) or <span class="tex-font-style-tt">N</span> (no), telling you if variety $a_c$ is one of the last $k$ varieties of coffee in his memory.</p></li><li> To reset the memory of your friend, in a separate line output the single letter <span class="tex-font-style-tt">R</span> <span class="tex-font-style-bf">in upper case</span>. You can do this operation at most $30\ 000$ times.</li><li> When you determine the number $d$ of different coffee varieties, output<p><span class="tex-font-style-tt">! $d$</span></p></li></ul><p>In case your query is invalid, you asked more than $\frac{3n^2}{2k}$ queries of type <span class="tex-font-style-tt">?</span> or you asked more than $30\ 000$ queries of type <span class="tex-font-style-tt">R</span>, the program will print the letter <span class="tex-font-style-tt">E</span> and will finish interaction. You will receive a <span class="tex-font-style-bf">Wrong Answer</span> verdict. Make sure to exit immediately to avoid getting other verdicts.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-bf">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hack format</span></p><p>The first line should contain the word <span class="tex-font-style-tt">fixed</span></p><p>The second line should contain two integers $n$ and $k$, separated by space ($1 \le k \le n \le 1024$, $k$ and $n$ are powers of two).</p><p>It must hold that $\dfrac{3n^2}{2k} \le 15\ 000$.</p><p>The third line should contain $n$ integers $a_1, a_2, \ldots, a_n$, separated by spaces ($1 \le a_i \le n$).</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \le k \le n \le 1024$, $k$ and $n$ are powers of two).</p><p>It is guaranteed that $\dfrac{3n^2}{2k} \le 15\ 000$.</p>





```input1
4 2
N
N
Y
N
N
N
N
```




```input2
8 8
N
N
N
N
Y
Y
```




```output1
? 1
? 2
? 3
? 4
R
? 4
? 1
? 2
! 3
```




```output2
? 2
? 6
? 4
? 5
? 2
? 5
! 6
```



## Note

<p>In the first example, the array is $a = [1, 4, 1, 3]$. The city produces $3$ different varieties of coffee ($1$, $3$ and $4$).</p><p>The successive varieties of coffee tasted by your friend are $1, 4, \textbf{1}, 3, 3, 1, 4$ (bold answers correspond to <span class="tex-font-style-tt">Y</span> answers). Note that between the two <span class="tex-font-style-tt">? 4</span> asks, there is a reset memory request <span class="tex-font-style-tt">R</span>, so the answer to the second <span class="tex-font-style-tt">? 4</span> ask is <span class="tex-font-style-tt">N</span>. Had there been no reset memory request, the answer to the second <span class="tex-font-style-tt">? 4</span> ask is <span class="tex-font-style-tt">Y</span>.</p><p>In the second example, the array is $a = [1, 2, 3, 4, 5, 6, 6, 6]$. The city produces $6$ different varieties of coffee.</p><p>The successive varieties of coffee tasted by your friend are $2, 6, 4, 5, \textbf{2}, \textbf{5}$.</p>
