## Description

<div><p>Ruritania is a country with a very badly maintained road network, which is not exactly good news for lorry drivers that constantly have to do deliveries. In fact, when roads are maintained, they become <span class="tex-font-style-bf">one-way</span>. It turns out that it is sometimes impossible to get from one town to another in a legal way – however, we know that all towns are <span class="tex-font-style-bf">reachable</span>, though <span class="tex-font-style-bf">illegally</span>!</p><p>Fortunately for us, the police tend to be very corrupt and they will allow a lorry driver to break the rules and drive in the wrong direction provided they receive ‘a small gift’. There is one patrol car for every road and they will request 1000 Ruritanian dinars when a driver drives in the wrong direction. However, being greedy, every time a patrol car notices the same driver breaking the rule, they will charge <span class="tex-font-style-bf">double</span> the amount of money they requested the previous time on that particular road.</p><p>Borna is a lorry driver that managed to figure out this bribing pattern. As part of his job, he has to make <span class="tex-span"><i>K</i></span> stops in some towns all over Ruritania and he has to make these stops in a certain order. There are <span class="tex-span"><i>N</i></span> towns (enumerated from 1 to <span class="tex-span"><i>N</i></span>) in Ruritania and Borna’s initial location is the capital city i.e. town 1. He happens to know which ones out of the <span class="tex-span"><i>N</i> - 1</span> roads in Ruritania are currently unidirectional, but he is unable to compute the least amount of money he needs to prepare for bribing the police. Help Borna by providing him with an answer and you will be richly rewarded.</p></div><div class="input-specification"><p>The first line contains <span class="tex-span"><i>N</i></span>, the number of towns in Ruritania. The following <span class="tex-span"><i>N</i> - 1</span> lines contain information regarding individual roads between towns. A road is represented by a tuple of integers (<span class="tex-span"><i>a</i></span>,<span class="tex-span"><i>b</i></span>,<span class="tex-span"><i>x</i></span>), which are separated with a single whitespace character. The numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> represent the cities connected by this particular road, and x is either 0 or 1: 0 means that the road is bidirectional, 1 means that only the <span class="tex-span"><i>a</i> → <i>b</i></span> direction is legal. The next line contains <span class="tex-span"><i>K</i></span>, the number of stops Borna has to make. The final line of input contains K positive integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, …, <i>s</i><sub class="lower-index"><i>K</i></sub></span>: the towns Borna has to visit.</p><ul> <li> <span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">1 ≤ <i>K</i> ≤ 10<sup class="upper-index">6</sup></span> </li><li> <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>N</i></span> for all roads </li><li> <img align="middle" class="tex-formula" src="file://bCmlRESm.png" style="max-width: 100.0%;max-height: 100.0%;"> for all roads </li><li> <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>N</i></span> for all <span class="tex-span">1 ≤ <i>i</i> ≤ <i>K</i></span> </li></ul></div><div class="output-specification"><p>The output should contain a single number: the least amount of thousands of Ruritanian dinars Borna should allocate for bribes, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains <span class="tex-span"><i>N</i></span>, the number of towns in Ruritania. The following <span class="tex-span"><i>N</i> - 1</span> lines contain information regarding individual roads between towns. A road is represented by a tuple of integers (<span class="tex-span"><i>a</i></span>,<span class="tex-span"><i>b</i></span>,<span class="tex-span"><i>x</i></span>), which are separated with a single whitespace character. The numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> represent the cities connected by this particular road, and x is either 0 or 1: 0 means that the road is bidirectional, 1 means that only the <span class="tex-span"><i>a</i> → <i>b</i></span> direction is legal. The next line contains <span class="tex-span"><i>K</i></span>, the number of stops Borna has to make. The final line of input contains K positive integers <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, …, <i>s</i><sub class="lower-index"><i>K</i></sub></span>: the towns Borna has to visit.</p><ul> <li> <span class="tex-span">1 ≤ <i>N</i> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">1 ≤ <i>K</i> ≤ 10<sup class="upper-index">6</sup></span> </li><li> <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>N</i></span> for all roads </li><li> <img align="middle" class="tex-formula" src="file://bCmlRESm.png" style="max-width: 100.0%;max-height: 100.0%;"> for all roads </li><li> <span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ <i>N</i></span> for all <span class="tex-span">1 ≤ <i>i</i> ≤ <i>K</i></span> </li></ul>

## Output

<p>The output should contain a single number: the least amount of thousands of Ruritanian dinars Borna should allocate for bribes, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
5
1 2 0
2 3 0
5 1 1
3 4 1
5
5 4 5 2 2

```




```output1
4

```



## Note

<p>Borna first takes the route <span class="tex-span">1 → 5</span> and has to pay 1000 dinars. After that, he takes the route <span class="tex-span">5 → 1 → 2 → 3 → 4</span> and pays nothing this time. However, when he has to return via <span class="tex-span">4 → 3 → 2 → 1 → 5</span>, he needs to prepare 3000 (1000+2000) dinars. Afterwards, getting to 2 via <span class="tex-span">5 → 1 → 2</span> will cost him nothing. Finally, he doesn't even have to leave town 2 to get to 2, so there is no need to prepare any additional bribe money. Hence he has to prepare 4000 dinars in total.</p>
