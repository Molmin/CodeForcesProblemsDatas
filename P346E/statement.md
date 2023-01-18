## Description

<div><p><span class="tex-font-style-underline"> In Doodle Jump the aim is to guide a four-legged creature called "The Doodler" up a never-ending series of platforms without falling. — Wikipedia. </span></p><p>It is a very popular game and xiaodao likes it very much. One day when playing the game she wondered whether there exists a platform that the doodler couldn't reach due to the limits of its jumping ability. Consider the following problem.</p><p>There are <span class="tex-span"><i>n</i></span> platforms. The height of the <span class="tex-span"><i>x</i></span>-th (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>) platform is <span class="tex-span"><i>a</i>·<i>x</i></span> mod <span class="tex-span"><i>p</i></span>, where <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>p</i></span> are positive co-prime integers. The maximum possible height of a Doodler's jump is <span class="tex-span"><i>h</i></span>. That is, it can jump from height <span class="tex-span"><i>h</i><sub class="lower-index">1</sub></span> to height <span class="tex-span"><i>h</i><sub class="lower-index">2</sub></span> (<span class="tex-span"><i>h</i><sub class="lower-index">1</sub> &lt; <i>h</i><sub class="lower-index">2</sub></span>) if <span class="tex-span"><i>h</i><sub class="lower-index">2</sub> - <i>h</i><sub class="lower-index">1</sub> ≤ <i>h</i></span>. Initially, the Doodler is on the ground, the height of which is 0. The question is whether it can reach the highest platform or not.</p><p>For example, when <span class="tex-span"><i>a</i> = 7</span>, <span class="tex-span"><i>n</i> = 4</span>, <span class="tex-span"><i>p</i> = 12</span>, <span class="tex-span"><i>h</i> = 2</span>, the heights of the platforms are <span class="tex-span">7</span>, <span class="tex-span">2</span>, <span class="tex-span">9</span>, <span class="tex-span">4</span> as in the picture below. With the first jump the Doodler can jump to the platform at height <span class="tex-span">2</span>, with the second one the Doodler can jump to the platform at height <span class="tex-span">4</span>, but then it can't jump to any of the higher platforms. So, it can't reach the highest platform.</p><center> <img class="tex-graphics" src="file://Agbszlpe.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>User xiaodao thought about the problem for a long time but didn't solve it, so she asks you for help. Also, she has a lot of instances of the problem. Your task is solve all of these instances.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 10<sup class="upper-index">4</sup>)</span> — the number of problem instances. Each of the next <span class="tex-span"><i>t</i></span> lines contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>n</i> &lt; <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>h</i> ≤ 10<sup class="upper-index">9</sup></span>). It's guaranteed that <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>p</i></span> are co-prime.</p></div><div class="output-specification"><p>For each problem instance, if the Doodler can reach the highest platform, output "<span class="tex-font-style-tt">YES</span>", otherwise output "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 10<sup class="upper-index">4</sup>)</span> — the number of problem instances. Each of the next <span class="tex-span"><i>t</i></span> lines contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>n</i> &lt; <i>p</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">0 ≤ <i>h</i> ≤ 10<sup class="upper-index">9</sup></span>). It's guaranteed that <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>p</i></span> are co-prime.</p>

## Output

<p>For each problem instance, if the Doodler can reach the highest platform, output "<span class="tex-font-style-tt">YES</span>", otherwise output "<span class="tex-font-style-tt">NO</span>".</p>





```input1
3
7 4 12 2
7 1 9 4
7 4 12 3

```




```output1
NO
NO
YES

```


