## Description

<div><p>In Berland recently a new collection of toys went on sale. This collection consists of <span class="tex-span">10<sup class="upper-index">9</sup></span> types of toys, numbered with integers from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span>. A toy from the new collection of the <span class="tex-span"><i>i</i></span>-th type costs <span class="tex-span"><i>i</i></span> bourles.</p><p>Tania has managed to collect <span class="tex-span"><i>n</i></span> different types of toys <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> from the new collection. Today is Tanya's birthday, and her mother decided to spend no more than <span class="tex-span"><i>m</i></span> bourles on the gift to the daughter. Tanya will choose several different types of toys from the new collection as a gift. Of course, she does not want to get a type of toy which she already has.</p><p>Tanya wants to have as many distinct types of toys in her collection as possible as the result. The new collection is too diverse, and Tanya is too little, so she asks you to help her in this.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of types of toys that Tanya already has and the number of bourles that her mom is willing to spend on buying new toys.</p><p>The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the types of toys that Tanya already has.</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of different types of toys that Tanya should choose so that the number of different types of toys in her collection is maximum possible. Of course, the total cost of the selected toys should not exceed <span class="tex-span"><i>m</i></span>.</p><p>In the second line print <span class="tex-span"><i>k</i></span> distinct space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the types of toys that Tanya should choose.</p><p>If there are multiple answers, you may print any of them. Values of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> can be printed in any order.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the number of types of toys that Tanya already has and the number of bourles that her mom is willing to spend on buying new toys.</p><p>The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the types of toys that Tanya already has.</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>k</i></span>&nbsp;— the number of different types of toys that Tanya should choose so that the number of different types of toys in her collection is maximum possible. Of course, the total cost of the selected toys should not exceed <span class="tex-span"><i>m</i></span>.</p><p>In the second line print <span class="tex-span"><i>k</i></span> distinct space-separated integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the types of toys that Tanya should choose.</p><p>If there are multiple answers, you may print any of them. Values of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> can be printed in any order.</p>





```input1
3 7
1 3 4

```




```input2
4 14
4 6 12 8

```




```output1
2
2 5 

```




```output2
4
7 2 3 1

```



## Note

<p>In the first sample mom should buy two toys: one toy of the <span class="tex-span">2</span>-nd type and one toy of the <span class="tex-span">5</span>-th type. At any other purchase for <span class="tex-span">7</span> bourles (assuming that the toys of types <span class="tex-span">1</span>, <span class="tex-span">3</span> and <span class="tex-span">4</span> have already been bought), it is impossible to buy two and more toys.</p>
