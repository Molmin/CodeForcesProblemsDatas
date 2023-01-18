## Description

<div><p>Programmer Sasha is a student at MIPT (Moscow Institute of Physics and Technology) and he needs to make a laboratory work to pass his finals.</p><p>A laboratory unit is a plane with standard coordinate axes marked on it. Physicists from Moscow Institute of Physics and Technology charged the axes by large electric charges: axis <span class="tex-span"><i>X</i></span> is positive and axis <span class="tex-span"><i>Y</i></span> is negative.</p><p>Experienced laboratory worker marked <span class="tex-span"><i>n</i></span> points with integer coordinates <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> on the plane and stopped the time. Sasha should use "atomic tweezers" to place elementary particles in these points. He has an unlimited number of electrons (negatively charged elementary particles) and protons (positively charged elementary particles). He can put either an electron or a proton at each marked point. As soon as all marked points are filled with particles, laboratory worker will turn on the time again and the particles will come in motion and after some time they will stabilize in equilibrium. The objective of the laboratory work is to arrange the particles in such a way, that the diameter of the resulting state (the maximum distance between the pairs of points of the set) is as small as possible.</p><p>Since Sasha is a programmer, he naively thinks that all the particles will simply "fall" into their projections on the corresponding axes: electrons will fall on axis <span class="tex-span"><i>X</i></span>, while protons will fall on axis <span class="tex-span"><i>Y</i></span>. As we are programmers too, we will consider the same model as Sasha. That is, a <span class="tex-font-style-bf">particle gets from point <span class="tex-span">(<i>x</i>, <i>y</i>)</span> to point <span class="tex-span">(<i>x</i>, 0)</span> if it is an electron and to point <span class="tex-span">(0, <i>y</i>)</span> if it is a proton.</span></p><p>As the laboratory has high background radiation and Sasha takes care of his laptop, he did not take it with him, and now he can't write a program that computes the minimum possible diameter of the resulting set. Therefore, you will have to do it for him.</p><p>Print a <span class="tex-font-style-bf">square</span> of the minimum possible diameter of the set.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of points marked on the plane.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th point. It is guaranteed that no two points coincide.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the square of the minimum possible diameter of the set.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of points marked on the plane.</p><p>Each of the next <span class="tex-span"><i>n</i></span> lines contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">8</sup> ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— the coordinates of the <span class="tex-span"><i>i</i></span>-th point. It is guaranteed that no two points coincide.</p>

## Output

<p>Print a single integer&nbsp;— the square of the minimum possible diameter of the set.</p>





```input1
3
1 10
1 20
1 30

```




```input2
2
1 10
10 1

```




```output1
0

```




```output2
2

```



## Note

<p>In the first sample Sasha puts electrons at all points, all particles eventually fall at a single point <span class="tex-span">(1, 0)</span>.</p><p>In the second sample Sasha puts an electron at point <span class="tex-span">(1, 10)</span>, and a proton at point <span class="tex-span">(10, 1)</span>. The result is a set of two points <span class="tex-span">(1, 0)</span> and <span class="tex-span">(0, 1)</span>, which has a diameter of <img align="middle" class="tex-formula" src="file://DiELc6HK.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
