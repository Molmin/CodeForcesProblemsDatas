## Description

<div><p>Linda likes to change her hair color from time to time, and would be pleased if her boyfriend Archie would notice the difference between the previous and the new color. Archie always comments on Linda's hair color if and only if he notices a difference — so Linda always knows whether Archie has spotted the difference or not.</p><p>There is a new hair dye series in the market where all available colors are numbered by integers from $1$ to $N$ such that a smaller difference of the numerical values also means less visual difference.</p><p>Linda assumes that for these series there should be some <span class="tex-font-style-it">critical color difference</span> $C$ ($1 \le C \le N$) for which Archie will notice color difference between the current color $\mathrm{color}_{\mathrm{new}}$ and the previous color $\mathrm{color}_{\mathrm{prev}}$ if $\left|\mathrm{color}_{\mathrm{new}} - \mathrm{color}_{\mathrm{prev}}\right| \ge C$ and will not if $\left|\mathrm{color}_{\mathrm{new}} - \mathrm{color}_{\mathrm{prev}}\right| &lt; C$.</p><p>Now she has bought $N$ sets of hair dye from the new series — one for each of the colors from $1$ to $N$, and is ready to set up an experiment. Linda will change her hair color on a regular basis and will observe Archie's reaction — whether he will notice the color change or not. Since for the proper dye each set should be used completely, each hair color can be obtained no more than once.</p><p>Before the experiment, Linda was using a dye from a different series which is not compatible with the new one, so for the clearness of the experiment Archie's reaction to the first used color is meaningless.</p><p>Her aim is to find the precise value of $C$ in a limited number of dyes. Write a program which finds the value of $C$ by experimenting with the given $N$ colors and observing Archie's reactions to color changes.</p></div><div><h2>Interaction</h2><p>This is an interactive task. In the beginning you are given a single integer $T$ ($1 \leq T \leq 100$), the number of cases in the test.</p><p>For each test case, the input first contains a single integer — the value of $N$ ($1 &lt; N \le 10^{18}$). The value of $C$ is kept secret by the grading system.</p><p>Then your program should make queries writing output in the following format: "<span class="tex-font-style-tt">? $P$</span>", where $P$ is an integer ($1 \le P \le N$) denoting the next color used. For each query the grading system gives an answer in the next line of the input. The answer is $1$ if Archie notices the color difference between the last two colors and $0$ otherwise. No two queries should have the same $P$ value.</p><p>When your program determines $C$, it should output its value in the following format: "<span class="tex-font-style-tt">= $C$</span>". The grading system will not respond to this output and will proceed with the next test case.</p><p>Your program may use <span class="tex-font-style-bf">at most 64</span> queries "<span class="tex-font-style-tt">?</span>" for each test case to find the correct value of $C$.</p><p>To establish proper communication between your program and the grading system, you should flush the output stream after each query.</p><center> $$\begin{array}{ll} \text{Language} &amp; \text{Command} \\ \hline \text{C++} &amp; \texttt{std::cout }\texttt{&lt;}\texttt{&lt;}\texttt{ std::endl;} \\ \text{Java} &amp; \texttt{System.out.flush();} \\ \text{Python} &amp; \texttt{sys.stdout.flush()} \end{array}$$ Flush commands </center><p>Note that <span class="tex-font-style-tt">std::endl</span> writes a newline and flushes the stream.</p><p>It is possible to receive an "Output isn't correct" outcome even after printing a correct answer, if task constraints were violated during the communication. Violating the communication protocol itself may result in an "Execution killed" outcome.</p><p>Submitting user tests requires specifying an input file with the testcase parameters. The format of the input file is "<span class="tex-font-style-tt">$T$</span>" in the first line, and then "<span class="tex-font-style-tt">$N$ $C$</span>" on a single line for each of the $T$ cases.</p></div><div><h2>Scoring</h2><p>Subtasks: </p><ol> <li> (9 points) $N \le 64$ </li><li> (13 points) $N \le 125$ </li><li> (21 points) $N \le 1000$ </li><li> (24 points) $N \le 10^9$ </li><li> (33 points) No further constraints. </li></ol></div>





```input1
1

7

1

1

0

0

1
```




```output1
? 2

? 7

? 4

? 1

? 5

= 4
```



## Note

<p>Comments to the example input line by line: </p><ol> <li> $N = 7$. </li><li> Answer to the first query is meaningless (can also be $0$). </li><li> $C \leq 5$. </li><li> $3 &lt; C \leq 5$. It would be wise to check difference $4$. However, this can not be done in the next query since $4 + 4 = 8$ and $4 - 4 = 0$ both are outside the allowed interval $1 \le P \le 7$. </li><li> $3 &lt; C \leq 5$. </li><li> $3 &lt; C \leq 4$. Therefore, $C = 4$. </li></ol>
