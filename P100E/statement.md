## Description

<div><p>There are <span class="tex-span"><i>n</i></span> lamps in a line. The lamps are numbered <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right. There are also <span class="tex-span"><i>n</i></span> keys. When key number <span class="tex-span"><i>i</i></span> is pressed, all lamps number <span class="tex-span"><i>x</i></span> such that <span class="tex-span"><i>i</i>|<i>x</i></span> change their state.</p><p>For two integer numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, we say <span class="tex-span"><i>a</i>|<i>b</i></span> if and only if there exists an integer <span class="tex-span"><i>c</i></span> such that <span class="tex-span"><i>a</i> × <i>c</i> = <i>b</i></span>.</p><p>Amirali likes to play with the keys. He randomly pressed <span class="tex-span"><i>k</i></span> keys and wants to know the final state of the lamps. Help him by writing a <span class="tex-font-style-underline">Pike</span> piece of code to solve this task.</p></div><div class="input-specification"><p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span>, the number of lamps (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The following line contains <span class="tex-span"><i>n</i></span> words. The <span class="tex-span"><i>i</i></span>-th word describes the initial state of lamp number <span class="tex-span"><i>i</i></span> (see samples for details).</p><p>The following line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>), the number of times a key is pressed. Then in the next line come <span class="tex-span"><i>k</i></span> integers in range <span class="tex-span">[1, <i>n</i>]</span> which are the numbers of the pressed keys.</p></div><div class="output-specification"><p>Write <span class="tex-span"><i>n</i></span> words to output. Describe the final state of the lamps. See samples for more details.</p></div>

## Input

<p>The first line of input contains a single integer <span class="tex-span"><i>n</i></span>, the number of lamps (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The following line contains <span class="tex-span"><i>n</i></span> words. The <span class="tex-span"><i>i</i></span>-th word describes the initial state of lamp number <span class="tex-span"><i>i</i></span> (see samples for details).</p><p>The following line contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">4</sup></span>), the number of times a key is pressed. Then in the next line come <span class="tex-span"><i>k</i></span> integers in range <span class="tex-span">[1, <i>n</i>]</span> which are the numbers of the pressed keys.</p>

## Output

<p>Write <span class="tex-span"><i>n</i></span> words to output. Describe the final state of the lamps. See samples for more details.</p>





```input1
2
off off
2
1 2

```




```input2
3
off off on
6
1 1 1 1 2 2

```




```output1
on off 

```




```output2
off off on 

```


