## Description

<div><p>Bearland has <span class="tex-span"><i>n</i></span> cities, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. There are <span class="tex-span"><i>m</i></span> bidirectional roads. The <span class="tex-span"><i>i</i></span>-th road connects two distinct cities <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. No two roads connect the same pair of cities. It's possible to get from any city to any other city (using one or more roads).</p><p>The distance between cities <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> is defined as the minimum number of roads used to travel between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>.</p><p>Limak is a grizzly bear. He is a criminal and your task is to catch him, or at least to try to catch him. You have only two days (today and tomorrow) and after that Limak is going to hide forever.</p><p>Your main weapon is BCD (Bear Criminal Detector). Where you are in some city, you can use BCD and it tells you the distance between you and a city where Limak currently is. Unfortunately, BCD can be used only once a day.</p><p>You don't know much about Limak's current location. You assume that he is in one of <span class="tex-span"><i>n</i></span> cities, chosen uniformly at random (each city with probability <img align="middle" class="tex-formula" src="file://rpuRBe9E.png" style="max-width: 100.0%;max-height: 100.0%;">). You decided for the following plan:</p><ol> <li> Choose one city and use BCD there. <ul> <li> After using BCD you can try to catch Limak (but maybe it isn't a good idea). In this case you choose one city and check it. You win if Limak is there. Otherwise, Limak becomes more careful and you will never catch him (you loose). </li></ul> </li><li> Wait <span class="tex-span">24</span> hours to use BCD again. You know that Limak will change his location during that time. In detail, he will choose uniformly at random one of roads from his initial city, and he will use the chosen road, going to some other city. </li><li> Tomorrow, you will again choose one city and use BCD there. </li><li> Finally, you will try to catch Limak. You will choose one city and check it. You will win if Limak is there, and loose otherwise. </li></ol><p>Each time when you choose one of cities, you can choose any of <span class="tex-span"><i>n</i></span> cities. Let's say it isn't a problem for you to quickly get somewhere.</p><p>What is the probability of finding Limak, if you behave optimally?</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 400</span>, <img align="middle" class="tex-formula" src="file://LWe9Bfiv.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of cities and the number of roads, respectively.</p><p>Then, <span class="tex-span"><i>m</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— cities connected by the <span class="tex-span"><i>i</i></span>-th road.</p><p>No two roads connect the same pair of cities. It's possible to get from any city to any other city.</p></div><div class="output-specification"><p>Print one real number&nbsp;— the probability of finding Limak, if you behave optimally. Your answer will be considered correct if its absolute error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <span class="tex-span">|<i>a</i> - <i>b</i>| ≤ 10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 400</span>, <img align="middle" class="tex-formula" src="file://LWe9Bfiv.png" style="max-width: 100.0%;max-height: 100.0%;">)&nbsp;— the number of cities and the number of roads, respectively.</p><p>Then, <span class="tex-span"><i>m</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>)&nbsp;— cities connected by the <span class="tex-span"><i>i</i></span>-th road.</p><p>No two roads connect the same pair of cities. It's possible to get from any city to any other city.</p>

## Output

<p>Print one real number&nbsp;— the probability of finding Limak, if you behave optimally. Your answer will be considered correct if its absolute error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct if <span class="tex-span">|<i>a</i> - <i>b</i>| ≤ 10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
3 3
1 2
1 3
2 3

```




```input2
5 4
1 2
3 1
5 1
1 4

```




```input3
4 4
1 2
1 3
2 3
1 4

```




```input4
5 5
1 2
2 3
3 4
4 5
1 5

```




```output1
0.833333333333

```




```output2
1.000000000000

```




```output3
0.916666666667

```




```output4
0.900000000000

```



## Note

<p>In the first sample test, there are three cities and there is a road between every pair of cities. Let's analyze one of optimal scenarios.</p><ol> <li> Use BCD in city <span class="tex-span">1</span>. <ul> <li> With probability <img align="middle" class="tex-formula" src="file://s3ib748W.png" style="max-width: 100.0%;max-height: 100.0%;"> Limak is in this city and BCD tells you that the distance is <span class="tex-span">0</span>. You should try to catch him now and you win for sure. </li><li> With probability <img align="middle" class="tex-formula" src="file://HdB10EOY.png" style="max-width: 100.0%;max-height: 100.0%;"> the distance is <span class="tex-span">1</span> because Limak is in city <span class="tex-span">2</span> or city <span class="tex-span">3</span>. In this case you should wait for the second day. </li></ul> </li><li> You wait and Limak moves to some other city. <ul> <li> There is probability <img align="middle" class="tex-formula" src="file://GkcesvxA.png" style="max-width: 100.0%;max-height: 100.0%;"> that Limak was in city <span class="tex-span">2</span> and then went to city <span class="tex-span">3</span>. </li><li> <img align="middle" class="tex-formula" src="file://UXhlUXp0.png" style="max-width: 100.0%;max-height: 100.0%;"> that he went from <span class="tex-span">2</span> to <span class="tex-span">1</span>. </li><li> <img align="middle" class="tex-formula" src="file://JO9m6c5M.png" style="max-width: 100.0%;max-height: 100.0%;"> that he went from <span class="tex-span">3</span> to <span class="tex-span">2</span>. </li><li> <img align="middle" class="tex-formula" src="file://06rR51lL.png" style="max-width: 100.0%;max-height: 100.0%;"> that he went from <span class="tex-span">3</span> to <span class="tex-span">1</span>. </li></ul> </li><li> Use BCD again in city <span class="tex-span">1</span> (though it's allowed to use it in some other city). <ul> <li> If the distance is <span class="tex-span">0</span> then you're sure Limak is in this city (you win). </li><li> If the distance is <span class="tex-span">1</span> then Limak is in city <span class="tex-span">2</span> or city <span class="tex-span">3</span>. Then you should guess that he is in city <span class="tex-span">2</span> (guessing city <span class="tex-span">3</span> would be fine too). </li></ul> </li></ol><p>You loose only if Limak was in city <span class="tex-span">2</span> first and then he moved to city <span class="tex-span">3</span>. The probability of loosing is <img align="middle" class="tex-formula" src="file://EYZEg9z2.png" style="max-width: 100.0%;max-height: 100.0%;">. The answer is <img align="middle" class="tex-formula" src="file://zTbH4fE2.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
