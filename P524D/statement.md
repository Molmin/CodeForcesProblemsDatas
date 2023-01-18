## Description

<div><p>Polycarpus got an internship in one well-known social network. His test task is to count the number of unique users who have visited a social network during the day. Polycarpus was provided with information on all user requests for this time period. For each query, we know its time... and nothing else, because Polycarpus has already accidentally removed the user IDs corresponding to the requests from the database. Thus, it is now impossible to determine whether any two requests are made by the same person or by different people.</p><p>But wait, something is still known, because that day a record was achieved — <span class="tex-span"><i>M</i></span> simultaneous users online! In addition, Polycarpus believes that if a user made a request at second <span class="tex-span"><i>s</i></span>, then he was online for <span class="tex-span"><i>T</i></span> seconds after that, that is, at seconds <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>s</i> + 1</span>, <span class="tex-span"><i>s</i> + 2</span>, ..., <span class="tex-span"><i>s</i> + <i>T</i> - 1</span>. So, the user's time online can be calculated as the union of time intervals of the form <span class="tex-span">[<i>s</i>, <i>s</i> + <i>T</i> - 1]</span> over all times <span class="tex-span"><i>s</i></span> of requests from him.</p><p>Guided by these thoughts, Polycarpus wants to assign a user ID to each request so that:</p><ul> <li> the number of different users online did not exceed <span class="tex-span"><i>M</i></span> at any moment, </li><li> at some second the number of distinct users online reached value <span class="tex-span"><i>M</i></span>, </li><li> the total number of users (the number of distinct identifiers) was as much as possible. </li></ul><p>Help Polycarpus cope with the test.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>M</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>M</i> ≤ 20 000</span>, <span class="tex-span">1 ≤ <i>T</i> ≤ 86400</span>) — the number of queries, the record number of online users and the time when the user was online after a query was sent. Next <span class="tex-span"><i>n</i></span> lines contain the times of the queries in the format "hh:mm:ss", where hh are hours, mm are minutes, ss are seconds. The times of the queries follow in the non-decreasing order, some of them can coincide. It is guaranteed that all the times and even all the segments of type <span class="tex-span">[<i>s</i>, <i>s</i> + <i>T</i> - 1]</span> are within one 24-hour range (from 00:00:00 to 23:59:59). </p></div><div class="output-specification"><p>In the first line print number <span class="tex-span"><i>R</i></span> — the largest possible number of distinct users. The following <span class="tex-span"><i>n</i></span> lines should contain the user IDs for requests in the same order in which the requests are given in the input. User IDs must be integers from <span class="tex-span">1</span> to <span class="tex-span"><i>R</i></span>. The requests of the same user must correspond to the same identifiers, the requests of distinct users must correspond to distinct identifiers. If there are multiple solutions, print any of them. If there is no solution, print "No solution" (without the quotes).</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>M</i></span> and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>M</i> ≤ 20 000</span>, <span class="tex-span">1 ≤ <i>T</i> ≤ 86400</span>) — the number of queries, the record number of online users and the time when the user was online after a query was sent. Next <span class="tex-span"><i>n</i></span> lines contain the times of the queries in the format "hh:mm:ss", where hh are hours, mm are minutes, ss are seconds. The times of the queries follow in the non-decreasing order, some of them can coincide. It is guaranteed that all the times and even all the segments of type <span class="tex-span">[<i>s</i>, <i>s</i> + <i>T</i> - 1]</span> are within one 24-hour range (from 00:00:00 to 23:59:59). </p>

## Output

<p>In the first line print number <span class="tex-span"><i>R</i></span> — the largest possible number of distinct users. The following <span class="tex-span"><i>n</i></span> lines should contain the user IDs for requests in the same order in which the requests are given in the input. User IDs must be integers from <span class="tex-span">1</span> to <span class="tex-span"><i>R</i></span>. The requests of the same user must correspond to the same identifiers, the requests of distinct users must correspond to distinct identifiers. If there are multiple solutions, print any of them. If there is no solution, print "No solution" (without the quotes).</p>





```input1
4 2 10
17:05:53
17:05:58
17:06:01
22:39:47

```




```input2
1 2 86400
00:00:00

```




```output1
3
1
2
2
3

```




```output2
No solution

```



## Note

<p>Consider the first sample. The user who sent the first request was online from 17:05:53 to 17:06:02, the user who sent the second request was online from 17:05:58 to 17:06:07, the user who sent the third request, was online from 17:06:01 to 17:06:10. Thus, these IDs cannot belong to three distinct users, because in that case all these users would be online, for example, at 17:06:01. That is impossible, because <span class="tex-span"><i>M</i> = 2</span>. That means that some two of these queries belonged to the same user. One of the correct variants is given in the answer to the sample. For it user <span class="tex-span">1</span> was online from 17:05:53 to 17:06:02, user <span class="tex-span">2</span> — from 17:05:58 to 17:06:10 (he sent the second and third queries), user <span class="tex-span">3</span> — from 22:39:47 to 22:39:56.</p><p>In the second sample there is only one query. So, only one user visited the network within the 24-hour period and there couldn't be two users online on the network simultaneously. (The time the user spent online is the union of time intervals for requests, so users who didn't send requests could not be online in the network.) </p>
