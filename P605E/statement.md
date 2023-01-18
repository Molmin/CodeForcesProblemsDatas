## Description

<div><p>The scientists have recently discovered wormholes&nbsp;— objects in space that allow to travel very long distances between galaxies and star systems. </p><p>The scientists know that there are <span class="tex-span"><i>n</i></span> galaxies within reach. You are in the galaxy number <span class="tex-span">1</span> and you need to get to the galaxy number <span class="tex-span"><i>n</i></span>. To get from galaxy <span class="tex-span"><i>i</i></span> to galaxy <span class="tex-span"><i>j</i></span>, you need to fly onto a wormhole <span class="tex-span">(<i>i</i>, <i>j</i>)</span> and in exactly one galaxy day you will find yourself in galaxy <span class="tex-span"><i>j</i></span>. </p><p>Unfortunately, the required wormhole is not always available. Every galaxy day they disappear and appear at random. However, the state of wormholes does not change within one galaxy day. A wormhole from galaxy <span class="tex-span"><i>i</i></span> to galaxy <span class="tex-span"><i>j</i></span> exists during each galaxy day taken separately with probability <span class="tex-span"><i>p</i><sub class="lower-index"><i>ij</i></sub></span>. You can always find out what wormholes exist at the given moment. At each moment you can either travel to another galaxy through one of wormholes that exist at this moment or you can simply wait for one galaxy day to see which wormholes will lead from your current position at the next day.</p><p>Your task is to find the expected value of time needed to travel from galaxy <span class="tex-span">1</span> to galaxy <span class="tex-span"><i>n</i></span>, if you act in the optimal way. It is guaranteed that this expected value exists.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of galaxies within reach.</p><p>Then follows a matrix of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns. Each element <span class="tex-span"><i>p</i><sub class="lower-index"><i>ij</i></sub></span> represents the probability that there is a wormhole from galaxy <span class="tex-span"><i>i</i></span> to galaxy <span class="tex-span"><i>j</i></span>. All the probabilities are given in percents and are integers. It is guaranteed that all the elements on the main diagonal are equal to <span class="tex-span">100</span>.</p></div><div class="output-specification"><p>Print a single real value&nbsp;— the expected value of the time needed to travel from galaxy <span class="tex-span">1</span> to galaxy <span class="tex-span"><i>n</i></span> if one acts in an optimal way. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://tGBhWmFW.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>)&nbsp;— the number of galaxies within reach.</p><p>Then follows a matrix of <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>n</i></span> columns. Each element <span class="tex-span"><i>p</i><sub class="lower-index"><i>ij</i></sub></span> represents the probability that there is a wormhole from galaxy <span class="tex-span"><i>i</i></span> to galaxy <span class="tex-span"><i>j</i></span>. All the probabilities are given in percents and are integers. It is guaranteed that all the elements on the main diagonal are equal to <span class="tex-span">100</span>.</p>

## Output

<p>Print a single real value&nbsp;— the expected value of the time needed to travel from galaxy <span class="tex-span">1</span> to galaxy <span class="tex-span"><i>n</i></span> if one acts in an optimal way. Your answer will be considered correct if its absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>. </p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://tGBhWmFW.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
3
100 50 50
0 100 80
0 0 100

```




```input2
2
100 30
40 100

```




```output1
1.750000000000000

```




```output2
3.333333333333333

```



## Note

<p>In the second sample the wormhole from galaxy <span class="tex-span">1</span> to galaxy <span class="tex-span">2</span> appears every day with probability equal to <span class="tex-span">0.3</span>. The expected value of days one needs to wait before this event occurs is <img align="middle" class="tex-formula" src="file://MUhYu9L9.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
