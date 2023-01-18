## Description

<div><p><span class="tex-font-style-it">The problem uses a simplified TCP/IP address model, please make sure you've read the statement attentively.</span></p><p>Polycarpus has found a job, he is a system administrator. One day he came across <span class="tex-span"><i>n</i></span> IP addresses. Each IP address is a 32 bit number, represented as a group of four 8-bit numbers (without leading zeroes), separated by dots. For example, the record <span class="tex-font-style-tt">0.255.1.123</span> shows a correct IP address and records <span class="tex-font-style-tt">0.256.1.123</span> and <span class="tex-font-style-tt">0.255.1.01</span> do not. In this problem an arbitrary group of four 8-bit numbers is a correct IP address.</p><p>Having worked as an administrator for some time, Polycarpus learned that if you know the IP address, you can use the subnet mask to get the address of the network that has this IP addess.</p><p>The <span class="tex-font-style-it">subnet mask</span> is an IP address that has the following property: if we write this IP address as a 32 bit string, that it is representable as "<span class="tex-font-style-tt">11...11000..000</span>". In other words, the subnet mask first has one or more one bits, and then one or more zero bits (overall there are 32 bits). For example, the IP address <span class="tex-font-style-tt">2.0.0.0</span> is not a correct subnet mask as its 32-bit record looks as <span class="tex-font-style-tt">00000010000000000000000000000000</span>.</p><p>To get the network address of the IP address, you need to perform the operation of the bitwise "<span class="tex-font-style-tt">and</span>" of the IP address and the subnet mask. For example, if the subnet mask is <span class="tex-font-style-tt">255.192.0.0</span>, and the IP address is <span class="tex-font-style-tt">192.168.1.2</span>, then the network address equals <span class="tex-font-style-tt">192.128.0.0</span>. In the bitwise "and" the result has a bit that equals 1 if and only if both operands have corresponding bits equal to one.</p><p>Now Polycarpus wants to find all networks to which his IP addresses belong. Unfortunately, Polycarpus lost subnet mask. Fortunately, Polycarpus remembers that his IP addresses belonged to exactly <span class="tex-span"><i>k</i></span> distinct networks. Help Polycarpus find the subnet mask, such that his IP addresses will belong to exactly <span class="tex-span"><i>k</i></span> distinct networks. If there are several such subnet masks, find the one whose bit record contains the least number of ones. If such subnet mask do not exist, say so.</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of IP addresses and networks. The next <span class="tex-span"><i>n</i></span> lines contain the IP addresses. It is guaranteed that all IP addresses are distinct.</p></div><div class="output-specification"><p>In a single line print the IP address of the subnet mask in the format that is described in the statement, if the required subnet mask exists. Otherwise, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of IP addresses and networks. The next <span class="tex-span"><i>n</i></span> lines contain the IP addresses. It is guaranteed that all IP addresses are distinct.</p>

## Output

<p>In a single line print the IP address of the subnet mask in the format that is described in the statement, if the required subnet mask exists. Otherwise, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
5 3
0.0.0.1
0.1.1.2
0.0.2.1
0.1.1.0
0.0.2.3

```




```input2
5 2
0.0.0.1
0.1.1.2
0.0.2.1
0.1.1.0
0.0.2.3

```




```input3
2 1
255.0.0.1
0.0.0.2

```




```output1
255.255.254.0
```




```output2
255.255.0.0
```




```output3
-1

```


