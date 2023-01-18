## Description

<div><p>Polycarpus works as a programmer in a start-up social network. His boss gave his a task to develop a mechanism for determining suggested friends. Polycarpus thought much about the task and came to the folowing conclusion. </p><p>Let's say that all friendship relationships in a social network are given as <span class="tex-span"><i>m</i></span> username pairs <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>. Each pair <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> means that users <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> are friends. Friendship is symmetric, that is, if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is friends with <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, then <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is also friends with <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. User <span class="tex-span"><i>y</i></span> is a <span class="tex-font-style-it">suggested friend</span> for user <span class="tex-span"><i>x</i></span>, if the following conditions are met:</p><ol> <li> <span class="tex-span"><i>x</i> ≠ <i>y</i></span>; </li><li> <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> aren't friends; </li><li> among all network users who meet the first two conditions, user <span class="tex-span"><i>y</i></span> has most of all common friends with user <span class="tex-span"><i>x</i></span>. User <span class="tex-span"><i>z</i></span> is a common friend of user <span class="tex-span"><i>x</i></span> and user <span class="tex-span"><i>y</i></span> <span class="tex-span">(<i>z</i> ≠ <i>x</i>, <i>z</i> ≠ <i>y</i>)</span>, if <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>z</i></span> are friends, and <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>z</i></span> are also friends. </li></ol><p>Your task is to help Polycarpus to implement a mechanism for determining suggested friends.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 5000)</span> — the number of pairs of friends in the social network. Next <span class="tex-span"><i>m</i></span> lines contain pairs of names of the users who are friends with each other. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated names <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>. The users' names are non-empty and consist of at most 20 uppercase and lowercase English letters. </p><p>It is guaranteed that each pair of friends occurs only once in the input. For example, the input can't contain <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>x</i></span> at the same time. It is guaranteed that distinct users have distinct names. It is guaranteed that each social network user has at least one friend. The last thing guarantees that each username occurs at least once in the input.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>n</i></span> — the number of network users. In next <span class="tex-span"><i>n</i></span> lines print the number of suggested friends for each user. In the <span class="tex-span"><i>i</i></span>-th line print the name of the user <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and the number of his suggested friends <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> after a space. </p><p>You can print information about the users in any order.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 5000)</span> — the number of pairs of friends in the social network. Next <span class="tex-span"><i>m</i></span> lines contain pairs of names of the users who are friends with each other. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated names <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(<i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>)</span>. The users' names are non-empty and consist of at most 20 uppercase and lowercase English letters. </p><p>It is guaranteed that each pair of friends occurs only once in the input. For example, the input can't contain <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>y</i></span>, <span class="tex-span"><i>x</i></span> at the same time. It is guaranteed that distinct users have distinct names. It is guaranteed that each social network user has at least one friend. The last thing guarantees that each username occurs at least once in the input.</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>n</i></span> — the number of network users. In next <span class="tex-span"><i>n</i></span> lines print the number of suggested friends for each user. In the <span class="tex-span"><i>i</i></span>-th line print the name of the user <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and the number of his suggested friends <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> after a space. </p><p>You can print information about the users in any order.</p>





```input1
5
Mike Gerald
Kate Mike
Kate Tank
Gerald Tank
Gerald David

```




```input2
4
valera vanya
valera edik
pasha valera
igor valera

```




```output1
5
Mike 1
Gerald 1
Kate 1
Tank 1
David 2

```




```output2
5
valera 0
vanya 3
edik 3
pasha 3
igor 3

```



## Note

<p>In the first test case consider user David. Users Mike and Tank have one common friend (Gerald) with David. User Kate has no common friends with David. That's why David's suggested friends are users Mike and Tank.</p>
