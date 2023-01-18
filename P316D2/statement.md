## Description

<div><p>Smart Beaver decided to be not only smart, but also a healthy beaver! And so he began to attend physical education classes at school X. In this school, physical education has a very creative teacher. One of his favorite warm-up exercises is throwing balls. Students line up. Each one gets a single ball in the beginning. The balls are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> (by the demand of the inventory commission).</p><center> <img class="tex-graphics" src="file://MFlojkf9.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script"> Figure 1. The initial position for <span class="tex-span"><i>n</i> = 5</span>. </span> </center><p>After receiving the balls the students perform the warm-up exercise. The exercise takes place in a few throws. For each throw the teacher chooses any two arbitrary different students who will participate in it. The selected students throw their balls to each other. Thus, after each throw the students remain in their positions, and the two balls are swapped.</p><center> <img class="tex-graphics" src="file://VbUINZOh.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-script"> Figure 2. The example of a throw. </span> </center><p>In this case there was a throw between the students, who were holding the <span class="tex-span">2</span>-nd and the <span class="tex-span">4</span>-th balls. Since the warm-up has many exercises, each of them can only continue for little time. Therefore, for each student we know the maximum number of throws he can participate in. For this lessons maximum number of throws will be <span class="tex-span">1</span> or <span class="tex-span">2</span>.</p><p>Note that after all phases of the considered exercise any ball can end up with any student. Smart Beaver decided to formalize it and introduced the concept of the "ball order". The ball order is a sequence of <span class="tex-span"><i>n</i></span> numbers that correspond to the order of balls in the line. The first number will match the number of the ball of the first from the left student in the line, the second number will match the ball of the second student, and so on. For example, in figure <span class="tex-span">2</span> the order of the balls was (<span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>, <span class="tex-span">5</span>), and after the throw it was (<span class="tex-span">1</span>, <span class="tex-span">4</span>, <span class="tex-span">3</span>, <span class="tex-span">2</span>, <span class="tex-span">5</span>). Smart beaver knows the number of students and for each student he knows the maximum number of throws in which he can participate. And now he is wondering: what is the number of distinct ways of ball orders by the end of the exercise.</p></div><div class="input-specification"><p>The first line contains a single number <span class="tex-span"><i>n</i></span> — the number of students in the line and the number of balls. The next line contains exactly <span class="tex-span"><i>n</i></span> space-separated integers. Each number corresponds to a student in the line (the <span class="tex-span"><i>i</i></span>-th number corresponds to the <span class="tex-span"><i>i</i></span>-th from the left student in the line) and shows the number of throws he can participate in.</p><p>The input limits for scoring 30 points are (subproblem D1): </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>. </li></ul><p>The input limits for scoring 70 points are (subproblems D1+D2): </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>. </li></ul><p>The input limits for scoring 100 points are (subproblems D1+D2+D3): </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 1000000</span>. </li></ul></div><div class="output-specification"><p>The output should contain a single integer — the number of variants of ball orders after the warm up exercise is complete. As the number can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div>

## Input

<p>The first line contains a single number <span class="tex-span"><i>n</i></span> — the number of students in the line and the number of balls. The next line contains exactly <span class="tex-span"><i>n</i></span> space-separated integers. Each number corresponds to a student in the line (the <span class="tex-span"><i>i</i></span>-th number corresponds to the <span class="tex-span"><i>i</i></span>-th from the left student in the line) and shows the number of throws he can participate in.</p><p>The input limits for scoring 30 points are (subproblem D1): </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>. </li></ul><p>The input limits for scoring 70 points are (subproblems D1+D2): </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>. </li></ul><p>The input limits for scoring 100 points are (subproblems D1+D2+D3): </p><ul> <li> <span class="tex-span">1 ≤ <i>n</i> ≤ 1000000</span>. </li></ul>

## Output

<p>The output should contain a single integer — the number of variants of ball orders after the warm up exercise is complete. As the number can be rather large, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p>





```input1
5
1 2 2 1 2

```




```input2
8
1 2 2 1 2 1 1 2

```




```output1
120

```




```output2
16800

```


