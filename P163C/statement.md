## Description

<div><p>Anton came to a chocolate factory. There he found a working conveyor and decided to run on it from the beginning to the end.</p><p>The conveyor is a looped belt with a total length of <span class="tex-span">2<i>l</i></span> meters, of which <span class="tex-span"><i>l</i></span> meters are located on the surface and are arranged in a straight line. The part of the belt which turns at any moment (the part which emerges from under the floor to the surface and returns from the surface under the floor) is assumed to be negligibly short.</p><p>The belt is moving uniformly at speed <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> meters per second. Anton will be moving on it in the same direction at the constant speed of <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> meters per second, so his speed relatively to the floor will be <span class="tex-span"><i>v</i><sub class="lower-index">1</sub> + <i>v</i><sub class="lower-index">2</sub></span> meters per second. Anton will neither stop nor change the speed or the direction of movement.</p><p>Here and there there are chocolates stuck to the belt (<span class="tex-span"><i>n</i></span> chocolates). They move together with the belt, and do not come off it. Anton is keen on the chocolates, but he is more keen to move forward. So he will pick up all the chocolates he will pass by, but nothing more. If a chocolate is at the beginning of the belt at the moment when Anton starts running, he will take it, and if a chocolate is at the end of the belt at the moment when Anton comes off the belt, he will leave it.</p><center> <img class="tex-graphics" src="file://P1XOB53k.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-size-script"> The figure shows an example with two chocolates. One is located   in the position <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = <i>l</i> - <i>d</i></span>, and is now on the top half of the belt, the second one   is in the position <span class="tex-span"><i>a</i><sub class="lower-index">2</sub> = 2<i>l</i> - <i>d</i></span>, and is now on the bottom half of the belt. </span> </center><p>You are given the positions of the chocolates relative to the initial start position of the belt <span class="tex-span">0 ≤ <i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub> &lt; 2<i>l</i></span>. The positions on the belt from <span class="tex-span">0</span> to <span class="tex-span"><i>l</i></span> correspond to the top, and from <span class="tex-span"><i>l</i></span> to <span class="tex-span">2<i>l</i></span> — to the the bottom half of the belt (see example). All coordinates are given in meters.</p><p>Anton begins to run along the belt at a random moment of time. This means that all possible positions of the belt at the moment he starts running are equiprobable. For each <span class="tex-span"><i>i</i></span> from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i></span> calculate the probability that Anton will pick up exactly <span class="tex-span"><i>i</i></span> chocolates.</p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>l</i>, <i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>) — the number of the chocolates, the length of the conveyor's visible part, the conveyor's speed and Anton's speed.</p><p>The second line contains a sequence of space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub> &lt; 2<i>l</i></span>) — the coordinates of the chocolates.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i> + 1</span> numbers (one per line): the probabilities that Anton picks up exactly <span class="tex-span"><i>i</i></span> chocolates, for each <span class="tex-span"><i>i</i></span> from <span class="tex-span">0</span> (the first line) to <span class="tex-span"><i>n</i></span> (the last line). The answer will be considered correct if each number will have absolute or relative error of at most than <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>v</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index">2</sub></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>l</i>, <i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub> ≤ 10<sup class="upper-index">9</sup></span>) — the number of the chocolates, the length of the conveyor's visible part, the conveyor's speed and Anton's speed.</p><p>The second line contains a sequence of space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>n</i></sub> &lt; 2<i>l</i></span>) — the coordinates of the chocolates.</p>

## Output

<p>Print <span class="tex-span"><i>n</i> + 1</span> numbers (one per line): the probabilities that Anton picks up exactly <span class="tex-span"><i>i</i></span> chocolates, for each <span class="tex-span"><i>i</i></span> from <span class="tex-span">0</span> (the first line) to <span class="tex-span"><i>n</i></span> (the last line). The answer will be considered correct if each number will have absolute or relative error of at most than <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
1 1 1 1
0

```




```input2
2 3 1 2
2 5

```




```output1
0.75000000000000000000
0.25000000000000000000

```




```output2
0.33333333333333331000
0.66666666666666663000
0.00000000000000000000

```



## Note

<p>In the first sample test Anton can pick up a chocolate if by the moment he starts running its coordinate is less than 0.5; but if by the moment the boy starts running the chocolate's coordinate is greater than or equal to 0.5, then Anton won't be able to pick it up. As all positions of the belt are equiprobable, the probability of picking up the chocolate equals <img align="middle" class="tex-formula" src="file://H5QMBZc7.png" style="max-width: 100.0%;max-height: 100.0%;">, and the probability of not picking it up equals <img align="middle" class="tex-formula" src="file://YWQAUQ3q.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
