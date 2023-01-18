## Description

<div><p>Vasya is choosing a laptop. The shop has <span class="tex-span"><i>n</i></span> laptops to all tastes.</p><p>Vasya is interested in the following properties: processor speed, ram and hdd. Vasya is a programmer and not a gamer which is why he is not interested in all other properties.</p><p>If all three properties of a laptop are <span class="tex-font-style-bf">strictly less</span> than those properties of some other laptop, then the first laptop is considered outdated by Vasya. Among all laptops Vasya does not consider outdated, he chooses the cheapest one.</p><p>There are very many laptops, which is why Vasya decided to write a program that chooses the suitable laptop. However, Vasya doesn't have his own laptop yet and he asks you to help him.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>).</p><p>Then follow <span class="tex-span"><i>n</i></span> lines. Each describes a laptop as <span class="tex-span"><i>speed</i></span> <span class="tex-span"><i>ram</i></span> <span class="tex-span"><i>hdd</i></span> <span class="tex-span"><i>cost</i></span>. Besides, </p><ul> <li> <span class="tex-span"><i>speed</i></span>, <span class="tex-span"><i>ram</i></span>, <span class="tex-span"><i>hdd</i></span> and <span class="tex-span"><i>cost</i></span> are integers </li><li> <span class="tex-span">1000 ≤ <i>speed</i> ≤ 4200</span> is the processor's speed in megahertz </li><li> <span class="tex-span">256 ≤ <i>ram</i> ≤ 4096</span> the RAM volume in megabytes </li><li> <span class="tex-span">1 ≤ <i>hdd</i> ≤ 500</span> is the HDD in gigabytes </li><li> <span class="tex-span">100 ≤ <i>cost</i> ≤ 1000</span> is price in tugriks </li></ul><p>All laptops have different prices.</p></div><div class="output-specification"><p>Print a single number — the number of a laptop Vasya will choose. The laptops are numbered with positive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order in which they are given in the input data.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>).</p><p>Then follow <span class="tex-span"><i>n</i></span> lines. Each describes a laptop as <span class="tex-span"><i>speed</i></span> <span class="tex-span"><i>ram</i></span> <span class="tex-span"><i>hdd</i></span> <span class="tex-span"><i>cost</i></span>. Besides, </p><ul> <li> <span class="tex-span"><i>speed</i></span>, <span class="tex-span"><i>ram</i></span>, <span class="tex-span"><i>hdd</i></span> and <span class="tex-span"><i>cost</i></span> are integers </li><li> <span class="tex-span">1000 ≤ <i>speed</i> ≤ 4200</span> is the processor's speed in megahertz </li><li> <span class="tex-span">256 ≤ <i>ram</i> ≤ 4096</span> the RAM volume in megabytes </li><li> <span class="tex-span">1 ≤ <i>hdd</i> ≤ 500</span> is the HDD in gigabytes </li><li> <span class="tex-span">100 ≤ <i>cost</i> ≤ 1000</span> is price in tugriks </li></ul><p>All laptops have different prices.</p>

## Output

<p>Print a single number — the number of a laptop Vasya will choose. The laptops are numbered with positive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order in which they are given in the input data.</p>





```input1
5
2100 512 150 200
2000 2048 240 350
2300 1024 200 320
2500 2048 80 300
2000 512 180 150

```




```output1
4
```



## Note

<p>In the third sample Vasya considers the first and fifth laptops outdated as all of their properties cannot match those of the third laptop. The fourth one is the cheapest among the laptops that are left. Thus, Vasya chooses the fourth laptop.</p>
