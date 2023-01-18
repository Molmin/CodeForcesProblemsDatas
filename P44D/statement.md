## Description

<div><p>In a far away galaxy there are <span class="tex-span"><i>n</i></span> inhabited planets, numbered with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. They are located at large distances from each other, that's why the communication between them was very difficult until on the planet number <span class="tex-span">1</span> a hyperdrive was invented. As soon as this significant event took place, <span class="tex-span"><i>n</i> - 1</span> spaceships were built on the planet number <span class="tex-span">1</span>, and those ships were sent to other planets to inform about the revolutionary invention. </p><p>Paradoxical thought it may be, but the hyperspace is represented as simple three-dimensional Euclidean space. The inhabited planets may be considered fixed points in it, and no two points coincide and no three points lie on the same straight line. The movement of a ship with a hyperdrive between two planets is performed along a straight line at the constant speed, the same for all the ships. That's why the distance in the hyperspace are measured in hyperyears (a ship with a hyperdrive covers a distance of <span class="tex-span"><i>s</i></span> hyperyears in <span class="tex-span"><i>s</i></span> years).</p><p>When the ship reaches an inhabited planet, the inhabitants of the planet dissemble it, make <span class="tex-span"><i>n</i> - 2</span> identical to it ships with a hyperdrive and send them to other <span class="tex-span"><i>n</i> - 2</span> planets (except for the one from which the ship arrived). The time to make a new ship compared to the time in which they move from one planet to another is so small that it can be disregarded. New ships are absolutely identical to the ones sent initially: they move at the same constant speed along a straight line trajectory and, having reached a planet, perform the very same mission, i.e. are dissembled to build new <span class="tex-span"><i>n</i> - 2</span> ships and send them to all the planets except for the one from which the ship arrived. Thus, the process of spreading the important news around the galaxy continues.</p><p>However the hyperdrive creators hurried to spread the news about their invention so much that they didn't study completely what goes on when two ships collide in the hyperspace. If two moving ships find themselves at one point, they provoke an explosion of colossal power, leading to the destruction of the galaxy!</p><p>Your task is to find the time the galaxy will continue to exist from the moment of the ships' launch from the first planet.</p></div><div class="input-specification"><p>The first line contains a number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 5000</span>) — the number of inhabited planets in the galaxy. The next <span class="tex-span"><i>n</i></span> lines contain integer coordinates of the planets in format "<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>). </p></div><div class="output-specification"><p>Print the single number — the solution to the task with an absolute or relative error not exceeding <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains a number <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 5000</span>) — the number of inhabited planets in the galaxy. The next <span class="tex-span"><i>n</i></span> lines contain integer coordinates of the planets in format "<span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span>" (<span class="tex-span"> - 10<sup class="upper-index">4</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>, <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>). </p>

## Output

<p>Print the single number — the solution to the task with an absolute or relative error not exceeding <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
4
0 0 0
0 0 1
0 1 0
1 0 0

```




```output1
1.7071067812

```


