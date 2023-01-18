## Description

<div><p>Polycarpus is a system administrator. There are two servers under his strict guidance — <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. To stay informed about the servers' performance, Polycarpus executes commands "<span class="tex-font-style-tt">ping a</span>" and "<span class="tex-font-style-tt">ping b</span>". Each ping command sends exactly ten packets to the server specified in the argument of the command. Executing a program results in two integers <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> <span class="tex-span">(<i>x</i> + <i>y</i> = 10;&nbsp;<i>x</i>, <i>y</i> ≥ 0)</span>. These numbers mean that <span class="tex-span"><i>x</i></span> packets successfully reached the corresponding server through the network and <span class="tex-span"><i>y</i></span> packets were lost.</p><p>Today Polycarpus has performed overall <span class="tex-span"><i>n</i></span> ping commands during his workday. Now for each server Polycarpus wants to know whether the server is "alive" or not. Polycarpus thinks that the server is "alive", if at least half of the packets that we send to this server reached it successfully along the network.</p><p>Help Polycarpus, determine for each server, whether it is "alive" or not by the given commands and their results.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 1000)</span> — the number of commands Polycarpus has fulfilled. Each of the following <span class="tex-span"><i>n</i></span> lines contains three integers — the description of the commands. The <span class="tex-span"><i>i</i></span>-th of these lines contains three space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2;&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≥ 0;&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub> + <i>y</i><sub class="lower-index"><i>i</i></sub> = 10)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then the <span class="tex-span"><i>i</i></span>-th command is "<span class="tex-font-style-tt">ping a</span>", otherwise the <span class="tex-span"><i>i</i></span>-th command is "<span class="tex-font-style-tt">ping b</span>". Numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> represent the result of executing this command, that is, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> packets reached the corresponding server successfully and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> packets were lost.</p><p>It is guaranteed that the input has at least one "<span class="tex-font-style-tt">ping a</span>" command and at least one "<span class="tex-font-style-tt">ping b</span>" command.</p></div><div class="output-specification"><p>In the first line print string "<span class="tex-font-style-tt">LIVE</span>" (without the quotes) if server <span class="tex-span"><i>a</i></span> is "alive", otherwise print "<span class="tex-font-style-tt">DEAD</span>" (without the quotes).</p><p>In the second line print the state of server <span class="tex-span"><i>b</i></span> in the similar format.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(2 ≤ <i>n</i> ≤ 1000)</span> — the number of commands Polycarpus has fulfilled. Each of the following <span class="tex-span"><i>n</i></span> lines contains three integers — the description of the commands. The <span class="tex-span"><i>i</i></span>-th of these lines contains three space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 2;&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≥ 0;&nbsp;<i>x</i><sub class="lower-index"><i>i</i></sub> + <i>y</i><sub class="lower-index"><i>i</i></sub> = 10)</span>. If <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>, then the <span class="tex-span"><i>i</i></span>-th command is "<span class="tex-font-style-tt">ping a</span>", otherwise the <span class="tex-span"><i>i</i></span>-th command is "<span class="tex-font-style-tt">ping b</span>". Numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> represent the result of executing this command, that is, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> packets reached the corresponding server successfully and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> packets were lost.</p><p>It is guaranteed that the input has at least one "<span class="tex-font-style-tt">ping a</span>" command and at least one "<span class="tex-font-style-tt">ping b</span>" command.</p>

## Output

<p>In the first line print string "<span class="tex-font-style-tt">LIVE</span>" (without the quotes) if server <span class="tex-span"><i>a</i></span> is "alive", otherwise print "<span class="tex-font-style-tt">DEAD</span>" (without the quotes).</p><p>In the second line print the state of server <span class="tex-span"><i>b</i></span> in the similar format.</p>





```input1
2
1 5 5
2 6 4

```




```input2
3
1 0 10
2 0 10
1 10 0

```




```output1
LIVE
LIVE

```




```output2
LIVE
DEAD

```



## Note

<p>Consider the first test case. There 10 packets were sent to server <span class="tex-span"><i>a</i></span>, 5 of them reached it. Therefore, at least half of all packets sent to this server successfully reached it through the network. Overall there were 10 packets sent to server <span class="tex-span"><i>b</i></span>, 6 of them reached it. Therefore, at least half of all packets sent to this server successfully reached it through the network.</p><p>Consider the second test case. There were overall 20 packages sent to server <span class="tex-span"><i>a</i></span>, 10 of them reached it. Therefore, at least half of all packets sent to this server successfully reached it through the network. Overall 10 packets were sent to server <span class="tex-span"><i>b</i></span>, 0 of them reached it. Therefore, less than half of all packets sent to this server successfully reached it through the network.</p>
