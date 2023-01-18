## Description

<div><p>Recently the construction of Berland collider has been completed. Collider can be represented as a long narrow tunnel that contains <span class="tex-span"><i>n</i></span> particles. We associate with collider 1-dimensional coordinate system, going from left to right. For each particle we know its coordinate and velocity at the moment of start of the collider. The velocities of the particles don't change after the launch of the collider. Berland scientists think that the big bang will happen at the first collision of particles, whose velocities differs in directions. Help them to determine how much time elapses after the launch of the collider before the big bang happens.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — amount of particles in the collider. Next <span class="tex-span"><i>n</i></span> lines contain description of particles. Each particle is described by two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span>) — coordinate and velocity respectively. All the coordinates are distinct. The particles are listed in order of increasing of coordinates. All the coordinates are in meters, and all the velocities — in meters per second. The negative velocity means that after the start of collider the particle will move to the left, and the positive — that the particle will move to the right.</p></div><div class="output-specification"><p>If there will be no big bang, output <span class="tex-font-style-tt">-1</span>. Otherwise output one number — how much time in seconds elapses after the launch of the collider before the big bang happens. Your answer must have a relative or absolute error less than <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>) — amount of particles in the collider. Next <span class="tex-span"><i>n</i></span> lines contain description of particles. Each particle is described by two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≠ 0</span>) — coordinate and velocity respectively. All the coordinates are distinct. The particles are listed in order of increasing of coordinates. All the coordinates are in meters, and all the velocities — in meters per second. The negative velocity means that after the start of collider the particle will move to the left, and the positive — that the particle will move to the right.</p>

## Output

<p>If there will be no big bang, output <span class="tex-font-style-tt">-1</span>. Otherwise output one number — how much time in seconds elapses after the launch of the collider before the big bang happens. Your answer must have a relative or absolute error less than <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
3
-5 9
0 1
5 -1

```




```input2
6
1 3
2 3
3 3
4 -3
5 -1
6 -100

```




```output1
1.00000000000000000000

```




```output2
0.02912621359223301065

```


