## Description

<div><p>As the guys fried the radio station facilities, the school principal gave them tasks as a punishment. Dustin's task was to add comments to nginx configuration for school's website. The school has <span class="tex-span"><i>n</i></span> servers. Each server has a name and an ip (names aren't necessarily unique, but ips are). Dustin knows the ip and name of each server. For simplicity, we'll assume that an nginx command is of form "<span class="tex-font-style-tt">command ip;</span>" where <span class="tex-font-style-tt">command</span> is a string consisting of English lowercase letter only, and <span class="tex-font-style-tt">ip</span> is the ip of one of school servers.</p><center> <img class="tex-graphics" src="file://lH7B8Irt.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Each ip is of form "<span class="tex-font-style-tt">a.b.c.d</span>" where <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> are non-negative integers less than or equal to <span class="tex-span">255</span> (with no leading zeros). The nginx configuration file Dustin has to add comments to has <span class="tex-span"><i>m</i></span> commands. Nobody ever memorizes the ips of servers, so to understand the configuration better, Dustin has to comment the name of server that the ip belongs to at the end of each line (after each command). More formally, if a line is "<span class="tex-font-style-tt">command ip;</span>" Dustin has to replace it with "<span class="tex-font-style-tt">command ip; #name</span>" where <span class="tex-font-style-tt">name</span> is the name of the server with ip equal to <span class="tex-font-style-tt">ip</span>.</p><p>Dustin doesn't know anything about nginx, so he panicked again and his friends asked you to do his task for him.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the names and ips of the servers. Each line contains a string <span class="tex-font-style-tt">name</span>, name of the server and a string <span class="tex-font-style-tt">ip</span>, ip of the server, separated by space (<span class="tex-span">1 ≤ |<i>name</i>| ≤ 10</span>, <span class="tex-span"><i>name</i></span> only consists of English lowercase letters). It is guaranteed that all ip are distinct.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the commands in the configuration file. Each line is of form "<span class="tex-font-style-tt">command ip;</span>" (<span class="tex-span">1 ≤ |<i>command</i>| ≤ 10</span>, <span class="tex-font-style-tt">command</span> only consists of English lowercase letters). It is guaranteed that ip belongs to one of the <span class="tex-span"><i>n</i></span> school servers.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines, the commands in the configuration file after Dustin did his task.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>).</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the names and ips of the servers. Each line contains a string <span class="tex-font-style-tt">name</span>, name of the server and a string <span class="tex-font-style-tt">ip</span>, ip of the server, separated by space (<span class="tex-span">1 ≤ |<i>name</i>| ≤ 10</span>, <span class="tex-span"><i>name</i></span> only consists of English lowercase letters). It is guaranteed that all ip are distinct.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain the commands in the configuration file. Each line is of form "<span class="tex-font-style-tt">command ip;</span>" (<span class="tex-span">1 ≤ |<i>command</i>| ≤ 10</span>, <span class="tex-font-style-tt">command</span> only consists of English lowercase letters). It is guaranteed that ip belongs to one of the <span class="tex-span"><i>n</i></span> school servers.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines, the commands in the configuration file after Dustin did his task.</p>





```input1
2 2
main 192.168.0.2
replica 192.168.0.1
block 192.168.0.1;
proxy 192.168.0.2;

```




```input2
3 5
google 8.8.8.8
codeforces 212.193.33.27
server 138.197.64.57
redirect 138.197.64.57;
block 8.8.8.8;
cf 212.193.33.27;
unblock 8.8.8.8;
check 138.197.64.57;

```




```output1
block 192.168.0.1; #replica
proxy 192.168.0.2; #main

```




```output2
redirect 138.197.64.57; #server
block 8.8.8.8; #google
cf 212.193.33.27; #codeforces
unblock 8.8.8.8; #google
check 138.197.64.57; #server

```


