## Description

<div><p>Vasya plays the Need For Brake. He plays because he was presented with a new computer wheel for birthday! Now he is sure that he will win the first place in the championship in his favourite racing computer game! </p><p><span class="tex-span"><i>n</i></span> racers take part in the championship, which consists of a number of races. After each race racers are arranged from place first to <span class="tex-span"><i>n</i></span>-th (no two racers share the same place) and first <span class="tex-span"><i>m</i></span> places are awarded. Racer gains <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> points for <span class="tex-span"><i>i</i></span>-th awarded place, which are added to total points, obtained by him for previous races. It is known that current summary score of racer <span class="tex-span"><i>i</i></span> is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> points. In the final standings of championship all the racers will be sorted in descending order of points. Racers with an equal amount of points are sorted by increasing of the name in lexicographical order.</p><p>Unfortunately, the championship has come to an end, and there is only one race left. Vasya decided to find out what the highest and lowest place he can take up as a result of the championship.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of racers. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — nick of the racer (nonempty string, which consist of no more than 20 lowercase Latin letters) and the racer's points (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). Racers are given in the arbitrary order.</p><p>The next line contains the number <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i></span>). Then <span class="tex-span"><i>m</i></span> nonnegative integer numbers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> follow. <span class="tex-span"><i>i</i></span>-th number is equal to amount of points for the <span class="tex-span"><i>i</i></span>-th awarded place (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The last line contains Vasya's racer nick.</p></div><div class="output-specification"><p>Output two numbers — the highest and the lowest place Vasya can take up as a result of the championship.</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of racers. Each of the next <span class="tex-span"><i>n</i></span> lines contains <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — nick of the racer (nonempty string, which consist of no more than 20 lowercase Latin letters) and the racer's points (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). Racers are given in the arbitrary order.</p><p>The next line contains the number <span class="tex-span"><i>m</i></span> (<span class="tex-span">0 ≤ <i>m</i> ≤ <i>n</i></span>). Then <span class="tex-span"><i>m</i></span> nonnegative integer numbers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> follow. <span class="tex-span"><i>i</i></span>-th number is equal to amount of points for the <span class="tex-span"><i>i</i></span>-th awarded place (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The last line contains Vasya's racer nick.</p>

## Output

<p>Output two numbers — the highest and the lowest place Vasya can take up as a result of the championship.</p>





```input1
3
teama 10
teamb 20
teamc 40
2
10 20
teama

```




```input2
2
teama 10
teamb 10
2
10 10
teamb

```




```output1
2 3
```




```output2
2 2
```


