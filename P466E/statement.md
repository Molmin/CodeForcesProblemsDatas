## Description

<div><p>There are <span class="tex-span"><i>n</i></span> employees working in company "X" (let's number them from 1 to <span class="tex-span"><i>n</i></span> for convenience). Initially the employees didn't have any relationships among each other. On each of <span class="tex-span"><i>m</i></span> next days one of the following events took place:</p><ul> <li> either employee <span class="tex-span"><i>y</i></span> became the boss of employee <span class="tex-span"><i>x</i></span> (at that, employee <span class="tex-span"><i>x</i></span> didn't have a boss before); </li><li> or employee <span class="tex-span"><i>x</i></span> gets a packet of documents and signs them; then he gives the packet to his boss. The boss signs the documents and gives them to his boss and so on (the last person to sign the documents sends them to the archive); </li><li> or comes a request of type "determine whether employee <span class="tex-span"><i>x</i></span> signs certain documents". </li></ul><p>Your task is to write a program that will, given the events, answer the queries of the described type. At that, it is guaranteed that throughout the whole working time the company didn't have cyclic dependencies.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of employees and the number of events. </p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains the description of one event (the events are given in the chronological order). The first number of the line determines the type of event <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 3)</span>. </p><ul> <li> If <span class="tex-span"><i>t</i> = 1</span>, then next follow two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>)</span> — numbers of the company employees. It is guaranteed that employee <span class="tex-span"><i>x</i></span> doesn't have the boss currently. </li><li> If <span class="tex-span"><i>t</i> = 2</span>, then next follow integer <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i>)</span> — the number of the employee who got a document packet. </li><li> If <span class="tex-span"><i>t</i> = 3</span>, then next follow two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>i</i> ≤ </span>[number of packets that have already been given]<span class="tex-span">)</span> — the employee and the number of the document packet for which you need to find out information. The document packets are numbered started from 1 in the chronological order. </li></ul><p>It is guaranteed that the input has at least one query of the third type.</p></div><div class="output-specification"><p>For each query of the third type print "<span class="tex-font-style-tt">YES</span>" if the employee signed the document package and "<span class="tex-font-style-tt">NO</span>" otherwise. Print all the words without the quotes.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of employees and the number of events. </p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains the description of one event (the events are given in the chronological order). The first number of the line determines the type of event <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 3)</span>. </p><ul> <li> If <span class="tex-span"><i>t</i> = 1</span>, then next follow two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(1 ≤ <i>x</i>, <i>y</i> ≤ <i>n</i>)</span> — numbers of the company employees. It is guaranteed that employee <span class="tex-span"><i>x</i></span> doesn't have the boss currently. </li><li> If <span class="tex-span"><i>t</i> = 2</span>, then next follow integer <span class="tex-span"><i>x</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i>)</span> — the number of the employee who got a document packet. </li><li> If <span class="tex-span"><i>t</i> = 3</span>, then next follow two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>i</i></span> <span class="tex-span">(1 ≤ <i>x</i> ≤ <i>n</i>;&nbsp;1 ≤ <i>i</i> ≤ </span>[number of packets that have already been given]<span class="tex-span">)</span> — the employee and the number of the document packet for which you need to find out information. The document packets are numbered started from 1 in the chronological order. </li></ul><p>It is guaranteed that the input has at least one query of the third type.</p>

## Output

<p>For each query of the third type print "<span class="tex-font-style-tt">YES</span>" if the employee signed the document package and "<span class="tex-font-style-tt">NO</span>" otherwise. Print all the words without the quotes.</p>





```input1
4 9
1 4 3
2 4
3 3 1
1 2 3
2 2
3 1 2
1 3 1
2 2
3 1 3

```




```output1
YES
NO
YES

```


