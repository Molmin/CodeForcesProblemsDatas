## Description

<div><p>Companies always have a lot of equipment, furniture and other things. All of them should be tracked. To do this, there is an inventory number assigned with each item. It is much easier to create a database by using those numbers and keep the track of everything.</p><p>During an audit, you were surprised to find out that the items are not numbered sequentially, and some items even share the same inventory number! There is an urgent need to fix it. You have chosen to make the numbers of the items sequential, starting with <span class="tex-span">1</span>. Changing a number is quite a time-consuming process, and you would like to make maximum use of the current numbering.</p><p>You have been given information on current inventory numbers for <span class="tex-span"><i>n</i></span> items in the company. Renumber items so that their inventory numbers form a <span class="tex-font-style-it">permutation</span> of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> by changing the number of as few items as possible. Let us remind you that a set of <span class="tex-span"><i>n</i></span> numbers forms a <span class="tex-font-style-it">permutation</span> if all the numbers are in the range from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and no two numbers are equal.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of items (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the initial inventory numbers of the items.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> numbers&nbsp;— the final inventory numbers of the items in the order they occur in the input. If there are multiple possible answers, you may print any of them.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span>&nbsp;— the number of items (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the initial inventory numbers of the items.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> numbers&nbsp;— the final inventory numbers of the items in the order they occur in the input. If there are multiple possible answers, you may print any of them.</p>





```input1
3
1 3 2

```




```input2
4
2 2 3 3

```




```input3
1
2

```




```output1
1 3 2 

```




```output2
2 1 3 4 

```




```output3
1 

```



## Note

<p>In the first test the numeration is already a permutation, so there is no need to change anything.</p><p>In the second test there are two pairs of equal numbers, in each pair you need to replace one number.</p><p>In the third test you need to replace <span class="tex-span">2</span> by <span class="tex-span">1</span>, as the numbering should start from one.</p>
