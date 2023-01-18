## Description

<div><p>One day two students, Grisha and Diana, found themselves in the university chemistry lab. In the lab the students found <span class="tex-span"><i>n</i></span> test tubes with mercury numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and decided to conduct an experiment.</p><p>The experiment consists of <span class="tex-span"><i>q</i></span> steps. On each step, one of the following actions occurs:</p><ol> <li> Diana pours all the contents from tube number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and then pours there exactly <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> liters of mercury. </li><li> Let's consider all the ways to add <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> liters of water into the tubes; for each way let's count the volume <span class="tex-font-style-bf">of liquid</span> (water and mercury) in the tube <span class="tex-font-style-bf">with water</span> with maximum amount of liquid; finally let's find the minimum among counted maximums. That is the number the students want to count. At that, the students don't actually pour the mercury. They perform calculations without changing the contents of the tubes. </li></ol><p>Unfortunately, the calculations proved to be too complex and the students asked you to help them. Help them conduct the described experiment.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of tubes ans the number of experiment steps. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the volume of mercury in the <span class="tex-span"><i>і</i></span>-th tube at the beginning of the experiment.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the game actions in the following format:</p><ul> <li> A line of form "<span class="tex-span">1</span> <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>" means an action of the first type (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </li><li> A line of form "<span class="tex-span">2</span> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>" means an action of the second type (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">15</sup></span>). </li></ul><p>It is guaranteed that there is at least one action of the second type. It is guaranteed that all numbers that describe the experiment are integers.</p></div><div class="output-specification"><p>For each action of the second type print the calculated value. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of tubes ans the number of experiment steps. The next line contains <span class="tex-span"><i>n</i></span> space-separated integers: <span class="tex-span"><i>h</i><sub class="lower-index">1</sub>, <i>h</i><sub class="lower-index">2</sub>, ..., <i>h</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> is the volume of mercury in the <span class="tex-span"><i>і</i></span>-th tube at the beginning of the experiment.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the game actions in the following format:</p><ul> <li> A line of form "<span class="tex-span">1</span> <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>" means an action of the first type (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>;&nbsp;0 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>). </li><li> A line of form "<span class="tex-span">2</span> <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>" means an action of the second type (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">15</sup></span>). </li></ul><p>It is guaranteed that there is at least one action of the second type. It is guaranteed that all numbers that describe the experiment are integers.</p>

## Output

<p>For each action of the second type print the calculated value. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
3 3
1 2 0
2 2
1 2 1
2 3

```




```input2
4 5
1 3 0 1
2 3
2 1
1 3 2
2 3
2 4

```




```output1
1.50000
1.66667

```




```output2
1.66667
1.00000
2.33333
2.66667

```


