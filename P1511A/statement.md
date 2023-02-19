## Description

<div><p>You are an upcoming movie director, and you have just released your first movie. You have also launched a simple review site with two buttons to press&nbsp;— upvote and downvote.</p><p>However, the site is not so simple on the inside. There are two servers, each with its separate counts for the upvotes and the downvotes.</p><p>$n$ reviewers enter the site one by one. Each reviewer is one of the following types: </p><ul> <li> type $1$: a reviewer has watched the movie, and they like it&nbsp;— they press the upvote button; </li><li> type $2$: a reviewer has watched the movie, and they dislike it&nbsp;— they press the downvote button; </li><li> type $3$: a reviewer hasn't watched the movie&nbsp;— they look at the current number of upvotes and downvotes of the movie on the server they are in and decide what button to press. If there are more downvotes than upvotes, then a reviewer downvotes the movie. Otherwise, they upvote the movie. </li></ul><p>Each reviewer votes on the movie exactly once.</p><p>Since you have two servers, you can actually manipulate the votes so that your movie gets as many upvotes as possible. When a reviewer enters a site, you know their type, and you can send them either to the first server or to the second one.</p><p>What is the maximum total number of upvotes you can gather over both servers if you decide which server to send each reviewer to?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 50$)&nbsp;— the number of reviewers.</p><p>The second line of each testcase contains $n$ integers $r_1, r_2, \dots, r_n$ ($1 \le r_i \le 3$)&nbsp;— the types of the reviewers in the same order they enter the site.</p></div><div class="output-specification"><p>For each testcase print a single integer&nbsp;— the maximum total number of upvotes you can gather over both servers if you decide which server to send each reviewer to.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 50$)&nbsp;— the number of reviewers.</p><p>The second line of each testcase contains $n$ integers $r_1, r_2, \dots, r_n$ ($1 \le r_i \le 3$)&nbsp;— the types of the reviewers in the same order they enter the site.</p>

## Output

<p>For each testcase print a single integer&nbsp;— the maximum total number of upvotes you can gather over both servers if you decide which server to send each reviewer to.</p>





```input1
4
1
2
3
1 2 3
5
1 1 1 1 1
3
3 3 2
```




```output1
0
2
5
2
```



## Note

<p>In the first testcase of the example you can send the only reviewer to either of the servers&nbsp;— they'll downvote anyway. The movie won't receive any upvotes.</p><p>In the second testcase of the example you can send all reviewers to the first server: </p><ul> <li> the first reviewer upvotes; </li><li> the second reviewer downvotes; </li><li> the last reviewer sees that the number of downvotes is not greater than the number of upvotes&nbsp;— upvote themselves. </li></ul><p>There are two upvotes in total. Alternatevely, you can send the first and the second reviewers to the first server and the last reviewer&nbsp;— to the second server: </p><ul> <li> the first reviewer upvotes on the first server; </li><li> the second reviewer downvotes on the first server; </li><li> the last reviewer sees no upvotes or downvotes on the second server&nbsp;— upvote themselves. </li></ul>
