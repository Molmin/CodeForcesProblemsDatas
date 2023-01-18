## Description

<div><p>In this problem you have to simulate the workflow of one-thread server. There are <span class="tex-span"><i>n</i></span> queries to process, the <span class="tex-span"><i>i</i></span>-th will be received at moment <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and needs to be processed for <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> units of time. All <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are guaranteed to be distinct.</p><p>When a query appears server may react in three possible ways: </p><ol> <li> If server is free and query queue is empty, then server immediately starts to process this query. </li><li> If server is busy and there are less than <span class="tex-span"><i>b</i></span> queries in the queue, then new query is added to the end of the queue. </li><li> If server is busy and there are already <span class="tex-span"><i>b</i></span> queries pending in the queue, then new query is just rejected and will never be processed. </li></ol><p>As soon as server finished to process some query, it picks new one from the queue (if it's not empty, of course). If a new query comes at some moment <span class="tex-span"><i>x</i></span>, and the server finishes to process another query at exactly the same moment, we consider that first query is picked from the queue and only then new query appears.</p><p>For each query find the moment when the server will finish to process it or print <span class="tex-font-style-tt">-1</span> if this query will be rejected.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>b</i> ≤ 200 000</span>)&nbsp;— the number of queries and the maximum possible size of the query queue.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines with queries descriptions (in chronological order). Each description consists of two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the moment of time when the <span class="tex-span"><i>i</i></span>-th query appears and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the time server needs to process it. It is guaranteed that <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i> - 1</sub> &lt; <i>t</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span"><i>i</i> &gt; 1</span>.</p></div><div class="output-specification"><p>Print the sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>e</i><sub class="lower-index">1</sub>, <i>e</i><sub class="lower-index">2</sub>, ..., <i>e</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span> is the moment the server will finish to process the <span class="tex-span"><i>i</i></span>-th query (queries are numbered in the order they appear in the input) or <span class="tex-span"> - 1</span> if the corresponding query will be rejected.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>b</i> ≤ 200 000</span>)&nbsp;— the number of queries and the maximum possible size of the query queue.</p><p>Then follow <span class="tex-span"><i>n</i></span> lines with queries descriptions (in chronological order). Each description consists of two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is the moment of time when the <span class="tex-span"><i>i</i></span>-th query appears and <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the time server needs to process it. It is guaranteed that <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i> - 1</sub> &lt; <i>t</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span"><i>i</i> &gt; 1</span>.</p>

## Output

<p>Print the sequence of <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>e</i><sub class="lower-index">1</sub>, <i>e</i><sub class="lower-index">2</sub>, ..., <i>e</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>e</i><sub class="lower-index"><i>i</i></sub></span> is the moment the server will finish to process the <span class="tex-span"><i>i</i></span>-th query (queries are numbered in the order they appear in the input) or <span class="tex-span"> - 1</span> if the corresponding query will be rejected.</p>





```input1
5 1
2 9
4 8
10 9
15 2
19 1

```




```input2
4 1
2 8
4 8
10 9
15 2

```




```output1
11 19 -1 21 22 

```




```output2
10 18 27 -1 

```



## Note

<p>Consider the first sample. </p><ol> <li> The server will start to process first query at the moment <span class="tex-span">2</span> and will finish to process it at the moment <span class="tex-span">11</span>. </li><li> At the moment <span class="tex-span">4</span> second query appears and proceeds to the queue. </li><li> At the moment <span class="tex-span">10</span> third query appears. However, the server is still busy with query <span class="tex-span">1</span>, <span class="tex-span"><i>b</i> = 1</span> and there is already query <span class="tex-span">2</span> pending in the queue, so third query is just rejected. </li><li> At the moment <span class="tex-span">11</span> server will finish to process first query and will take the second query from the queue. </li><li> At the moment <span class="tex-span">15</span> fourth query appears. As the server is currently busy it proceeds to the queue. </li><li> At the moment <span class="tex-span">19</span> two events occur simultaneously: server finishes to proceed the second query and the fifth query appears. As was said in the statement above, first server will finish to process the second query, then it will pick the fourth query from the queue and only then will the fifth query appear. As the queue is empty fifth query is proceed there. </li><li> Server finishes to process query number <span class="tex-span">4</span> at the moment <span class="tex-span">21</span>. Query number <span class="tex-span">5</span> is picked from the queue. </li><li> Server finishes to process query number <span class="tex-span">5</span> at the moment <span class="tex-span">22</span>. </li></ol>
