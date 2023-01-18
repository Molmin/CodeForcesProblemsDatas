## Description

<div><p>Wilbur the pig is tinkering with arrays again. He has the array <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> initially consisting of <span class="tex-span"><i>n</i></span> zeros. At one step, he can choose any index <span class="tex-span"><i>i</i></span> and either add <span class="tex-span">1</span> to all elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>, ... , <i>a</i><sub class="lower-index"><i>n</i></sub></span> or subtract <span class="tex-span">1</span> from all elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i> + 1</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. His goal is to end up with the array <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. </p><p>Of course, Wilbur wants to achieve this goal in the minimum number of steps and asks you to compute this value.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the length of the array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Initially <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span> for every position <span class="tex-span"><i>i</i></span>, so this array is not given in the input.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print the minimum number of steps that Wilbur needs to make in order to achieve <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span"><i>i</i></span>.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the length of the array <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Initially <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span> for every position <span class="tex-span"><i>i</i></span>, so this array is not given in the input.</p><p>The second line of the input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print the minimum number of steps that Wilbur needs to make in order to achieve <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i></sub></span> for all <span class="tex-span"><i>i</i></span>.</p>





```input1
5
1 2 3 4 5

```




```input2
4
1 2 2 1

```




```output1
5
```




```output2
3
```



## Note

<p>In the first sample, Wilbur may successively choose indices <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>, and <span class="tex-span">5</span>, and add <span class="tex-span">1</span> to corresponding suffixes.</p><p>In the second sample, Wilbur first chooses indices <span class="tex-span">1</span> and <span class="tex-span">2</span> and adds <span class="tex-span">1</span> to corresponding suffixes, then he chooses index <span class="tex-span">4</span> and subtract <span class="tex-span">1</span>.</p>
