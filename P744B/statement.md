## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem. In the interaction section below you will see the information about flushing the output.</span></p><p>In this problem, you will be playing a game with Hongcow. How lucky of you!</p><p>Hongcow has a hidden <span class="tex-span"><i>n</i></span> by <span class="tex-span"><i>n</i></span> matrix <span class="tex-span"><i>M</i></span>. Let <span class="tex-span"><i>M</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> denote the entry <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column of the matrix. The rows and columns are labeled from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>The matrix entries are between <span class="tex-span">0</span> and <span class="tex-span">10<sup class="upper-index">9</sup></span>. In addition, <span class="tex-span"><i>M</i><sub class="lower-index"><i>i</i>, <i>i</i></sub> = 0</span> for all valid <span class="tex-span"><i>i</i></span>. Your task is to find the minimum value along each row, excluding diagonal elements. Formally, for each <span class="tex-span"><i>i</i></span>, you must find <img align="middle" class="tex-formula" src="file://aNixaybp.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>To do this, you can ask Hongcow some questions.</p><p>A question consists of giving Hongcow a subset of distinct indices <span class="tex-span">{<i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>k</i></sub>}</span>, with <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>. Hongcow will respond with <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>i</i></span>-th integer will contain the minimum value of <span class="tex-span"><i>min</i><sub class="lower-index">1 ≤ <i>j</i> ≤ <i>k</i></sub><i>M</i><sub class="lower-index"><i>i</i>, <i>w</i><sub class="lower-index"><i>j</i></sub></sub></span>.</p><p>You may only ask Hongcow at most <span class="tex-span">20</span> questions&nbsp;— he thinks you only need that many questions answered.</p><p>When you are ready to answer, print out a single integer <span class="tex-span"> - 1</span> on its own line, then <span class="tex-span"><i>n</i></span> integers on the next line. The <span class="tex-span"><i>i</i></span>-th integer should be the minimum value in the <span class="tex-span"><i>i</i></span>-th row of the matrix, excluding the <span class="tex-span"><i>i</i></span>-th element. Do not forget to flush the final answer as well. Printing the answer does not count as asking a question.</p><p>You will get <span class="tex-font-style-tt">Wrong Answer</span> verdict if </p><ul> <li> Your question or answers are not in the format described in this statement. </li><li> You ask strictly more than <span class="tex-span">20</span> questions. </li><li> Your question contains duplicate indices. </li><li> The value of <span class="tex-span"><i>k</i></span> in your question does not lie in the range from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive. </li><li> Your final answer is not correct. </li></ul> You will get <span class="tex-font-style-tt">Idleness Limit Exceeded</span> if you don't print anything or if you forget to flush the output, including for the final answer (more info about flushing output below).</div><div class="input-specification"><p>The first line of input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1, 000</span>).</p></div><div class="output-specification"><p>To print the final answer, print out the string <span class="tex-font-style-tt">-1</span> on its own line. Then, the next line should contain <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>i</i></span>-th integer should be the minimum value of the <span class="tex-span"><i>i</i></span>-th row of the matrix, excluding elements on the diagonal. <span class="tex-font-style-bf">Do not forget to flush your answer!</span></p></div><div><h2>Interaction</h2><p>To ask a question, print out a single integer <span class="tex-span"><i>k</i></span> on its own line, denoting the size of your subset. Then, the next line should contain <span class="tex-span"><i>k</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ... <i>w</i><sub class="lower-index"><i>k</i></sub></span>. Note, you must flush your output to get a response.</p><p>Hongcow will respond by printing out a line with <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>i</i></span>-th integer in this line represents the minimum value of <span class="tex-span"><i>M</i><sub class="lower-index"><i>i</i>, <i>w</i><sub class="lower-index"><i>j</i></sub></sub></span> where <span class="tex-span"><i>j</i></span> is between <span class="tex-span">1</span> and <span class="tex-span"><i>k</i></span>.</p><p>You may only ask a question at most <span class="tex-span">20</span> times, otherwise, you will get <span class="tex-font-style-tt">Wrong Answer</span>.</p><p>To flush you can use (just after printing an integer and end-of-line): </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> See the documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacking</span> To hack someone, use the following format </p><pre class="verbatim"><br>n<br>M_{1,1} M_{1,2} ... M_{1,n}<br>M_{2,1} M_{2,2} ... M_{2,n}<br>...<br>M_{n,1} M_{n,2} ... M_{n,n}<br></pre><p>Of course, contestant programs will not be able to see this input.</p></div>

## Input

<p>The first line of input will contain a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1, 000</span>).</p>

## Output

<p>To print the final answer, print out the string <span class="tex-font-style-tt">-1</span> on its own line. Then, the next line should contain <span class="tex-span"><i>n</i></span> integers. The <span class="tex-span"><i>i</i></span>-th integer should be the minimum value of the <span class="tex-span"><i>i</i></span>-th row of the matrix, excluding elements on the diagonal. <span class="tex-font-style-bf">Do not forget to flush your answer!</span></p>





```input1
3
0 0 0
2 7 0
0 0 4
3 0 8
0 5 4
```




```input2
2
0 0
0 0
```




```output1
3
1 2 3
1
3
2
1 2
1
2
1
1
-1
2 5 4

```




```output2
1
2
1
1
-1
0 0
```



## Note

<p>In the first sample, Hongcow has the hidden matrix </p><pre class="verbatim"><br>[<br> [0, 3, 2],<br> [5, 0, 7],<br> [4, 8 ,0],<br>]<br></pre><p>Here is a more readable version demonstrating the interaction. The column on the left represents Hongcow, while the column on the right represents the contestant. </p><pre class="verbatim"><br>3<br>              3<br>              1 2 3<br>0 0 0<br>              1<br>              3<br>2 7 0<br>              2<br>              1 2<br>0 0 4<br>              1<br>              2<br>3 0 8<br>              1<br>              1<br>0 5 4<br>              -1<br>              2 5 4<br></pre><p>For the second sample, it is possible for off-diagonal elements of the matrix to be zero.</p>
