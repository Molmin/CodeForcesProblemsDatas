## Description

<div><p>Gennady is one of the best child dentists in Berland. Today <span class="tex-span"><i>n</i></span> children got an appointment with him, they lined up in front of his office.</p><p>All children love to cry loudly at the reception at the dentist. We enumerate the children with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> in the order they go in the line. Every child is associated with the value of his <span class="tex-font-style-it">cofidence</span> <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. The children take turns one after another to come into the office; each time the child that is the first in the line goes to the doctor.</p><p>While Gennady treats the teeth of the <span class="tex-span"><i>i</i></span>-th child, the child is crying with the volume of <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>. At that the <span class="tex-font-style-it">confidence</span> of the first child in the line is reduced by the amount of <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, the second one — by value <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub> - 1</span>, and so on. The children in the queue after the <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>-th child almost do not hear the crying, so their <span class="tex-font-style-it">confidence</span> remains unchanged.</p><p>If at any point in time the <span class="tex-font-style-it">confidence</span> of the <span class="tex-span"><i>j</i></span>-th child is less than zero, he begins to cry with the volume of <span class="tex-span"><i>d</i><sub class="lower-index"><i>j</i></sub></span> and leaves the line, running towards the exit, without going to the doctor's office. At this the <span class="tex-font-style-it">confidence</span> of all the children after the <span class="tex-span"><i>j</i></span>-th one in the line is reduced by the amount of <span class="tex-span"><i>d</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>All these events occur immediately one after the other in some order. Some cries may lead to other cries, causing a chain reaction. Once in the hallway it is quiet, the child, who is first in the line, goes into the doctor's office.</p><p>Help Gennady the Dentist to determine the numbers of kids, whose teeth he will cure. Print their numbers in the chronological order.</p></div><div class="input-specification"><p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4000</span>) — the number of kids in the line. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain three integers each <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the volume of the cry in the doctor's office, the volume of the cry in the hall and the <span class="tex-font-style-it">confidence</span> of the <span class="tex-span"><i>i</i></span>-th child.</p></div><div class="output-specification"><p>In the first line print number <span class="tex-span"><i>k</i></span> — the number of children whose teeth Gennady will cure.</p><p>In the second line print <span class="tex-span"><i>k</i></span> integers — the numbers of the children who will make it to the end of the line in the increasing order.</p></div>

## Input

<p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4000</span>) — the number of kids in the line. </p><p>Next <span class="tex-span"><i>n</i></span> lines contain three integers each <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub>, <i>d</i><sub class="lower-index"><i>i</i></sub>, <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) — the volume of the cry in the doctor's office, the volume of the cry in the hall and the <span class="tex-font-style-it">confidence</span> of the <span class="tex-span"><i>i</i></span>-th child.</p>

## Output

<p>In the first line print number <span class="tex-span"><i>k</i></span> — the number of children whose teeth Gennady will cure.</p><p>In the second line print <span class="tex-span"><i>k</i></span> integers — the numbers of the children who will make it to the end of the line in the increasing order.</p>





```input1
5
4 2 2
4 1 2
5 2 4
3 3 5
5 1 2

```




```input2
5
4 5 1
5 3 9
4 1 2
2 1 8
4 1 9

```




```output1
2
1 3
```




```output2
4
1 2 4 5
```



## Note

<p>In the first example, Gennady first treats the teeth of the first child who will cry with volume <span class="tex-span">4</span>. The confidences of the remaining children will get equal to <span class="tex-span"> - 2, 1, 3, 1</span>, respectively. Thus, the second child also cries at the volume of <span class="tex-span">1</span> and run to the exit. The confidence of the remaining children will be equal to <span class="tex-span">0, 2, 0</span>. Then the third child will go to the office, and cry with volume <span class="tex-span">5</span>. The other children won't bear this, and with a loud cry they will run to the exit.</p><p>In the second sample, first the first child goes into the office, he will cry with volume <span class="tex-span">4</span>. The confidence of the remaining children will be equal to <span class="tex-span">5,  - 1, 6, 8</span>. Thus, the third child will cry with the volume of <span class="tex-span">1</span> and run to the exit. The confidence of the remaining children will be equal to <span class="tex-span">5, 5, 7</span>. After that, the second child goes to the office and cry with the volume of <span class="tex-span">5</span>. The confidences of the remaining children will be equal to <span class="tex-span">0, 3</span>. Then the fourth child will go into the office and cry with the volume of <span class="tex-span">2</span>. Because of this the confidence of the fifth child will be <span class="tex-span">1</span>, and he will go into the office last.</p>
