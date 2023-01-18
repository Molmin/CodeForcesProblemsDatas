## Description

<div><p>Vasya is currently at a car rental service, and he wants to reach cinema. The film he has bought a ticket for starts in <span class="tex-span"><i>t</i></span> minutes. There is a straight road of length <span class="tex-span"><i>s</i></span> from the service to the cinema. Let's introduce a coordinate system so that the car rental service is at the point <span class="tex-span">0</span>, and the cinema is at the point <span class="tex-span"><i>s</i></span>.</p><p>There are <span class="tex-span"><i>k</i></span> gas stations along the road, and at each of them you can fill a car with any amount of fuel for free! Consider that this operation doesn't take any time, i.e. is carried out instantly.</p><p>There are <span class="tex-span"><i>n</i></span> cars in the rental service, <span class="tex-span"><i>i</i></span>-th of them is characterized with two integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the price of this car rent and the capacity of its fuel tank in liters. It's not allowed to fuel a car with more fuel than its tank capacity <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. All cars are completely fueled at the car rental service.</p><p>Each of the cars can be driven in one of two speed modes: normal or accelerated. In the normal mode a car covers <span class="tex-span">1</span> kilometer in <span class="tex-span">2</span> minutes, and consumes <span class="tex-span">1</span> liter of fuel. In the accelerated mode a car covers <span class="tex-span">1</span> kilometer in <span class="tex-span">1</span> minutes, but consumes <span class="tex-span">2</span> liters of fuel. The driving mode can be changed at any moment and any number of times.</p><p>Your task is to choose a car with minimum price such that Vasya can reach the cinema before the show starts, i.e. not later than in <span class="tex-span"><i>t</i></span> minutes. Assume that all cars are completely fueled initially.</p></div><div class="input-specification"><p>The first line contains four positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>s</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the number of cars at the car rental service, the number of gas stations along the road, the length of the road and the time in which the film starts. </p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two positive integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the price of the <span class="tex-span"><i>i</i></span>-th car and its fuel tank capacity.</p><p>The next line contains <span class="tex-span"><i>k</i></span> <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>g</i><sub class="lower-index">1</sub>, <i>g</i><sub class="lower-index">2</sub>, ..., <i>g</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index"><i>i</i></sub> ≤ <i>s</i> - 1</span>)&nbsp;— the positions of the gas stations on the road in arbitrary order.</p></div><div class="output-specification"><p>Print the minimum rent price of an appropriate car, i.e. such car that Vasya will be able to reach the cinema before the film starts (not later than in <span class="tex-span"><i>t</i></span> minutes). If there is no appropriate car, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains four positive integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">2 ≤ <i>s</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 2·10<sup class="upper-index">9</sup></span>)&nbsp;— the number of cars at the car rental service, the number of gas stations along the road, the length of the road and the time in which the film starts. </p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two positive integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the price of the <span class="tex-span"><i>i</i></span>-th car and its fuel tank capacity.</p><p>The next line contains <span class="tex-span"><i>k</i></span> <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>g</i><sub class="lower-index">1</sub>, <i>g</i><sub class="lower-index">2</sub>, ..., <i>g</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index"><i>i</i></sub> ≤ <i>s</i> - 1</span>)&nbsp;— the positions of the gas stations on the road in arbitrary order.</p>

## Output

<p>Print the minimum rent price of an appropriate car, i.e. such car that Vasya will be able to reach the cinema before the film starts (not later than in <span class="tex-span"><i>t</i></span> minutes). If there is no appropriate car, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
3 1 8 10
10 8
5 7
11 9
3

```




```input2
2 2 10 18
10 4
20 6
5 3

```




```output1
10

```




```output2
20

```



## Note

<p>In the first sample, Vasya can reach the cinema in time using the first or the third cars, but it would be cheaper to choose the first one. Its price is equal to <span class="tex-span">10</span>, and the capacity of its fuel tank is <span class="tex-span">8</span>. Then Vasya can drive to the first gas station in the accelerated mode in <span class="tex-span">3</span> minutes, spending <span class="tex-span">6</span> liters of fuel. After that he can full the tank and cover <span class="tex-span">2</span> kilometers in the normal mode in <span class="tex-span">4</span> minutes, spending <span class="tex-span">2</span> liters of fuel. Finally, he drives in the accelerated mode covering the remaining <span class="tex-span">3</span> kilometers in <span class="tex-span">3</span> minutes and spending <span class="tex-span">6</span> liters of fuel. </p>
