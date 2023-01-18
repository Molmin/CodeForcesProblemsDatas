## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem. In the interaction section below you will find the information about flushing the output.</span></p><p>The New Year tree of height <span class="tex-span"><i>h</i></span> is a perfect binary tree with vertices numbered <span class="tex-span">1</span> through <span class="tex-span">2<sup class="upper-index"><i>h</i></sup> - 1</span> in some order. In this problem we assume that <span class="tex-span"><i>h</i></span> is at least <span class="tex-span">2</span>. The drawing below shows one example New Year tree of height <span class="tex-span">3</span>:</p><center> <img class="tex-graphics" src="file://cUvlXkza.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Polar bears love decorating the New Year tree and Limak is no exception. To decorate the tree, he must first find its root, i.e. a vertex with exactly two neighbours (assuming that <span class="tex-span"><i>h</i> ≥ 2</span>). It won't be easy because Limak is a little bear and he doesn't even see the whole tree. Can you help him?</p><p>There are <span class="tex-span"><i>t</i></span> testcases. In each testcase, you should first read <span class="tex-span"><i>h</i></span> from the input. Then you can ask at most <span class="tex-span">16</span> questions of format "<span class="tex-font-style-tt">? x</span>" (without quotes), where <span class="tex-span"><i>x</i></span> is an integer between <span class="tex-span">1</span> and <span class="tex-span">2<sup class="upper-index"><i>h</i></sup> - 1</span>, inclusive. As a reply you will get the list of neighbours of vertex <span class="tex-span"><i>x</i></span> (more details in the "Interaction" section below). For example, for a tree on the drawing above after asking "<span class="tex-font-style-tt">? 1</span>" you would get a response with <span class="tex-span">3</span> neighbours: <span class="tex-span">4</span>, <span class="tex-span">5</span> and <span class="tex-span">7</span>. Your goal is to find the index of the root <span class="tex-span"><i>y</i></span> and print it in the format "<span class="tex-font-style-tt">! y</span>". You will be able to read <span class="tex-span"><i>h</i></span> for a next testcase only after printing the answer in a previous testcase and flushing the output.</p><p>Each tree is fixed from the beginning and it doesn't change during your questions.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 500</span>)&nbsp;— the number of testcases.</p><p>At the beginning of each testcase you should read from the input a single integer <span class="tex-span"><i>h</i></span> (<span class="tex-span">2 ≤ <i>h</i> ≤ 7</span>)&nbsp;— the height of the tree. You can't read the value of <span class="tex-span"><i>h</i></span> in a next testcase until you answer a previous testcase.</p></div><div><h2>Interaction</h2><p>To ask a question about neighbours of vertex <span class="tex-span"><i>x</i></span>, print "<span class="tex-font-style-tt">? x</span>" (without quotes) on a separate line. Note, you must print an end-of-line character after the last character of the line and flush your output to get a response.</p><p>The response will consist of two lines. The first line will contain a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 3</span>)&nbsp;— the number of neighbours of vertex <span class="tex-span"><i>x</i></span>. The second line will contain <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, ..., <i>t</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index">1</sub> &lt; ... &lt; <i>t</i><sub class="lower-index"><i>k</i></sub> ≤ 2<sup class="upper-index"><i>h</i></sup> - 1</span>)&nbsp;— indices of neighbours of vertex <span class="tex-span"><i>x</i></span>, gives in the increasing order.</p><p>After asking at most <span class="tex-span">16</span> questions you have to say <span class="tex-span"><i>y</i></span>&nbsp;— the index of the root. Print "<span class="tex-font-style-tt">! y</span>" (without quotes) and an end-of-line character, and flush the output.</p><p>Each tree is fixed from the beginning and it doesn't change during your questions.</p><p>You can get <span class="tex-font-style-tt">Idleness Limit Exceeded</span> if you don't print anything or if you forget to flush the output.</p><p>To flush you can use (just printing a query/answer and end-of-line): </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> See the documentation for other languages. </li></ul><p>In any moment if the program reads <span class="tex-span"><i>h</i> = 0</span> or <span class="tex-span"><i>k</i> = 0</span> it should immediately terminate normally (for example, calling exit(0)). It means that the system detected incorrect request/output from your program and printed 0 because if can't process your requests anymore. In this case you'll receive verdict "Wrong Answer", but if you ignore case <span class="tex-span"><i>h</i> = 0</span> or <span class="tex-span"><i>k</i> = 0</span> it could lead to "Runtime Error", "Time/Memory limit exceeded" or any other verdict because your program could read a trash from the closed input stream.</p><p><span class="tex-font-style-bf">Hacking</span>. To hack someone, use the following format:</p><p>The first line should contain a single integer <span class="tex-span"><i>t</i></span> equal to <span class="tex-span">1</span> (only one testcase is allowed in hacks). The second line should contain a single integer <span class="tex-span"><i>h</i></span>. Each of next <span class="tex-span">2<sup class="upper-index"><i>h</i></sup> - 2</span> lines should contain two distinct integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 2<sup class="upper-index"><i>h</i></sup> - 1</span>), denoting two nodes connected with an edge. The printed edges must form a perfect binary tree of height <span class="tex-span"><i>h</i></span>.</p><p>Of course, contestant programs will not be able to see this input.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 500</span>)&nbsp;— the number of testcases.</p><p>At the beginning of each testcase you should read from the input a single integer <span class="tex-span"><i>h</i></span> (<span class="tex-span">2 ≤ <i>h</i> ≤ 7</span>)&nbsp;— the height of the tree. You can't read the value of <span class="tex-span"><i>h</i></span> in a next testcase until you answer a previous testcase.</p>





```input1
1
3
3
4 5 7
2
1 2
1
2

```




```input2
2
2
1
3
2
1 2
2
1 2
4
3
3 12 13

```




```output1
? 1
? 5
? 6
! 5

```




```output2
? 1
? 3
? 3
! 3
? 6
! 1

```



## Note

<p>In the first sample, a tree corresponds to the drawing from the statement.</p><p>In the second sample, there are two two testcases. A tree in the first testcase has height <span class="tex-span">2</span> and thus <span class="tex-span">3</span> vertices. A tree in the second testcase has height <span class="tex-span">4</span> and thus <span class="tex-span">15</span> vertices. You can see both trees on the drawing below.</p><center> <img class="tex-graphics" src="file://LVirLflF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
