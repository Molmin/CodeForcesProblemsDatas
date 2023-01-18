## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>Jury has hidden a permutation <span class="tex-span"><i>p</i></span> of integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>. You know only the length <span class="tex-span"><i>n</i></span>. Remind that in permutation all integers are distinct.</p><p>Let <span class="tex-span"><i>b</i></span> be the inverse permutation for <span class="tex-span"><i>p</i></span>, i.e. <span class="tex-span"><i>p</i><sub class="lower-index"><i>b</i><sub class="lower-index"><i>i</i></sub></sub> = <i>i</i></span> for all <span class="tex-span"><i>i</i></span>. The only thing you can do is to ask <span class="tex-font-style-tt">xor</span> of elements <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span>, printing two indices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> (not necessarily distinct). As a result of the query with indices <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> you'll get the value <img align="middle" class="tex-formula" src="file://bsfy2ZYU.png" style="max-width: 100.0%;max-height: 100.0%;">, where <img align="middle" class="tex-formula" src="file://z7uNDo1H.png" style="max-width: 100.0%;max-height: 100.0%;"> denotes the <span class="tex-font-style-tt">xor</span> operation. You can find the description of <span class="tex-font-style-tt">xor</span> operation in notes.</p><p>Note that some permutations can remain indistinguishable from the hidden one, even if you make all possible <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> queries. You have to compute the number of permutations indistinguishable from the hidden one, and print one of such permutations, making no more than <span class="tex-span">2<i>n</i></span> queries.</p><p>The hidden permutation does not depend on your queries.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — the length of the hidden permutation. You should read this integer first.</p></div><div class="output-specification"><p>When your program is ready to print the answer, print three lines.</p><p>In the first line print "<span class="tex-font-style-tt">!</span>".</p><p>In the second line print single integer <span class="tex-span"><i>answers</i>_<i>cnt</i></span>&nbsp;— the number of permutations indistinguishable from the hidden one, including the hidden one. </p><p>In the third line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">0</sub>, <i>p</i><sub class="lower-index">1</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>, all <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> should be distinct)&nbsp;— one of the permutations indistinguishable from the hidden one.</p><p>Your program should terminate after printing the answer.</p></div><div><h2>Interaction</h2><p>To ask about <span class="tex-font-style-tt">xor</span> of two elements, print a string "<span class="tex-font-style-tt">? i j</span>", where <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> — are integers from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span> — the index of the permutation element and the index of the inverse permutation element you want to know the <span class="tex-font-style-tt">xor</span>-sum for. After that print a line break and make <span class="tex-font-style-tt">flush</span> operation.</p><p>After printing the query your program should read single integer&nbsp;— the value of <img align="middle" class="tex-formula" src="file://ZF9OCgbH.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p>For a permutation of length <span class="tex-span"><i>n</i></span> your program should make no more than <span class="tex-span">2<i>n</i></span> queries about <span class="tex-font-style-tt">xor</span>-sum. Note that printing answer doesn't count as a query. Note that you can't ask more than <span class="tex-span">2<i>n</i></span> questions. If you ask more than <span class="tex-span">2<i>n</i></span> questions or at least one incorrect question, your solution will get "<span class="tex-font-style-tt">Wrong answer</span>".</p><p>If at some moment your program reads <span class="tex-font-style-tt">-1</span> as an answer, it should immediately exit (for example, by calling <span class="tex-font-style-tt">exit(0)</span>). You will get "<span class="tex-font-style-tt">Wrong answer</span>" in this case, it means that you asked more than <span class="tex-span">2<i>n</i></span> questions, or asked an invalid question. If you ignore this, you can get other verdicts since your program will continue to read from a closed stream.</p><p>Your solution will get "<span class="tex-font-style-tt">Idleness Limit Exceeded</span>", if you don't print anything or forget to flush the output, including for the final answer .</p><p>To flush you can use (just after printing line break): </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> For other languages see the documentation. </li></ul><p><span class="tex-font-style-bf">Hacking</span></p><p>For hacking use the following format:</p><p><span class="tex-span"><i>n</i></span></p><p><span class="tex-span"><i>p</i><sub class="lower-index">0</sub></span> <span class="tex-span"><i>p</i><sub class="lower-index">1</sub></span> ... <span class="tex-span"><i>p</i><sub class="lower-index"><i>n</i> - 1</sub></span></p><p>Contestant programs will not be able to see this input.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>) — the length of the hidden permutation. You should read this integer first.</p>

## Output

<p>When your program is ready to print the answer, print three lines.</p><p>In the first line print "<span class="tex-font-style-tt">!</span>".</p><p>In the second line print single integer <span class="tex-span"><i>answers</i>_<i>cnt</i></span>&nbsp;— the number of permutations indistinguishable from the hidden one, including the hidden one. </p><p>In the third line print <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">0</sub>, <i>p</i><sub class="lower-index">1</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i> - 1</sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>, all <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> should be distinct)&nbsp;— one of the permutations indistinguishable from the hidden one.</p><p>Your program should terminate after printing the answer.</p>





```input1
3
0
0
3
2
3
2
```




```input2
4
2
3
2
0
2
3
2
0
```




```output1
? 0 0
? 1 1
? 1 2
? 0 2
? 2 1
? 2 0
!
1
0 1 2
```




```output2
? 0 1
? 1 2
? 2 3
? 3 3
? 3 2
? 2 1
? 1 0
? 0 0
!
2
3 1 2 0
```



## Note

<p><span class="tex-font-style-tt">xor</span> operation, or bitwise exclusive OR, is an operation performed over two integers, in which the <span class="tex-span"><i>i</i></span>-th digit in binary representation of the result is equal to <span class="tex-span">1</span> if and only if exactly one of the two integers has the <span class="tex-span"><i>i</i></span>-th digit in binary representation equal to <span class="tex-span">1</span>. For more information, see <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">here</a>.</p><p>In the first example <span class="tex-span"><i>p</i> = [0, 1, 2]</span>, thus <span class="tex-span"><i>b</i> = [0, 1, 2]</span>, the values <img align="middle" class="tex-formula" src="file://6Tbt37hh.png" style="max-width: 100.0%;max-height: 100.0%;"> are correct for the given <span class="tex-span"><i>i</i>, <i>j</i></span>. There are no other permutations that give the same answers for the given queries.</p><p>The answers for the queries are: </p><ul> <li> <img align="middle" class="tex-formula" src="file://jQprhBrx.png" style="max-width: 100.0%;max-height: 100.0%;">, </li><li> <img align="middle" class="tex-formula" src="file://nuHA4ZbM.png" style="max-width: 100.0%;max-height: 100.0%;">, </li><li> <img align="middle" class="tex-formula" src="file://8b35uMxS.png" style="max-width: 100.0%;max-height: 100.0%;">, </li><li> <img align="middle" class="tex-formula" src="file://NsmsLEtw.png" style="max-width: 100.0%;max-height: 100.0%;">, </li><li> <img align="middle" class="tex-formula" src="file://e36WDVVS.png" style="max-width: 100.0%;max-height: 100.0%;">, </li><li> <img align="middle" class="tex-formula" src="file://6gg7medI.png" style="max-width: 100.0%;max-height: 100.0%;">. </li></ul><p>In the second example <span class="tex-span"><i>p</i> = [3, 1, 2, 0]</span>, and <span class="tex-span"><i>b</i> = [3, 1, 2, 0]</span>, the values <img align="middle" class="tex-formula" src="file://hHl4Ex9Q.png" style="max-width: 100.0%;max-height: 100.0%;"> match for all pairs <span class="tex-span"><i>i</i>, <i>j</i></span>. But there is one more suitable permutation <span class="tex-span"><i>p</i> = [0, 2, 1, 3]</span>, <span class="tex-span"><i>b</i> = [0, 2, 1, 3]</span> that matches all <span class="tex-span"><i>n</i><sup class="upper-index">2</sup></span> possible queries as well. All other permutations do not match even the shown queries.</p>
