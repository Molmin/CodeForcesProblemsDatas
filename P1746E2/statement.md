## Description

<div><p><span class="tex-font-style-it">The only difference between this problem and the hard version is the maximum number of questions.</span></p><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>There is a hidden integer $1 \le x \le n$ which you have to find. In order to find it you can ask at most $\mathbf{53}$ questions.</p><p>In each question you can choose a non-empty integer set $S$ and ask if $x$ belongs to $S$ or not, after each question, if $x$ belongs to $S$, you'll receive "<span class="tex-font-style-tt">YES</span>", otherwise "<span class="tex-font-style-tt">NO</span>".</p><p>But the problem is that not all answers are necessarily true (some of them are joking), it's just guaranteed that for each two consecutive questions, at least one of them is answered correctly.</p><p>Additionally to the questions, you can make at most $2$ guesses for the answer $x$. Each time you make a guess, if you guess $x$ correctly, you receive "<span class="tex-font-style-tt">:)</span>" and your program should terminate, otherwise you'll receive "<span class="tex-font-style-tt">:(</span>".</p><p>As a part of the joking, we will <span class="tex-font-style-bf">not</span> fix the value of $x$ in the beginning. Instead, it can change throughout the interaction as long as all the previous responses are valid as described above.</p><p>Note that your answer guesses are always answered correctly. If you ask a question before and after a guess, at least one of these two questions is answered correctly, as normal.</p></div><div class="input-specification"><p>The only line of the input contains a single integer $n$ ($1 \le n \le 10^5$), the maximum possible value of $x$.</p></div><div><h2>Interaction</h2><p>For each question, if you want to ask about a set $S$, first print the character '<span class="tex-font-style-tt">?</span>', then print the size of $S$ and then print the elements of $S$ one by one. Each element should be an integer between $1$ and $n$, the elements must be distinct. After each question, read a string "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>", as explained in the statement. You can make at most $53$ such questions.</p><p>If you want to guess for $x$, first print the character '<span class="tex-font-style-tt">!</span>' and then print your guess. After each guess, read "<span class="tex-font-style-tt">:)</span>" or "<span class="tex-font-style-tt">:(</span>". If you guess $x$ correctly, the answer is "<span class="tex-font-style-tt">:)</span>" and your program should terminate immediately, otherwise you'll receive ":(". You can make at most $2$ such guesses.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacking is not allowed in this problem.</span></p></div>

## Input

<p>The only line of the input contains a single integer $n$ ($1 \le n \le 10^5$), the maximum possible value of $x$.</p>





```input1
6

NO

:(

NO

:)
```




```output1
? 5 1 2 5 4 3

! 6

? 4 1 2 3 4

! 5
```



## Note

<p>If the answer of the first question were correct, then $x$ would have been equal to $6$, but as we can see in the first guess, $6$ is not the answer.</p><p>So the answer of the first question is joking. As we know, the answer of at least one of our two questions is correct, since the answer of the first question was joking, the answer of the second question should be correct.</p><p>So we will understand that $x$ is not equal to $1, 2, 3$ or $4$, and we also knew that $x$ is not equal to $6$ either. Hence $x$ should be equal to $5$.</p>
