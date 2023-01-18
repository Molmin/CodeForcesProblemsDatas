## Description

<div><p>Petya has recently learned data structure named "Binary heap".</p><p>The heap he is now operating with allows the following operations: </p><ul> <li> put the given number into the heap; </li><li> get the value of the minimum element in the heap; </li><li> extract the minimum element from the heap; </li></ul><p>Thus, at any moment of time the heap contains several integers (possibly none), some of them might be equal.</p><p>In order to better learn this data structure Petya took an empty heap and applied some operations above to it. Also, he carefully wrote down all the operations and their results to his event log, following the format: </p><ul> <li> <span class="tex-font-style-tt">insert</span> <span class="tex-span"><i>x</i></span>&nbsp;— put the element with value <span class="tex-span"><i>x</i></span> in the heap; </li><li> <span class="tex-font-style-tt">getMin</span> <span class="tex-span"><i>x</i></span>&nbsp;— the value of the minimum element contained in the heap was equal to <span class="tex-span"><i>x</i></span>; </li><li> <span class="tex-font-style-tt">removeMin</span>&nbsp;— the minimum element was extracted from the heap (only one instance, if there were many). </li></ul><p>All the operations were correct, i.e. there was at least one element in the heap each time <span class="tex-font-style-tt">getMin</span> or <span class="tex-font-style-tt">removeMin</span> operations were applied.</p><p>While Petya was away for a lunch, his little brother Vova came to the room, took away some of the pages from Petya's log and used them to make paper boats.</p><p>Now Vova is worried, if he made Petya's sequence of operations inconsistent. For example, if one apply operations one-by-one in the order they are written in the event log, results of <span class="tex-font-style-tt">getMin</span> operations might differ from the results recorded by Petya, and some of <span class="tex-font-style-tt">getMin</span> or <span class="tex-font-style-tt">removeMin</span> operations may be incorrect, as the heap is empty at the moment they are applied.</p><p>Now Vova wants to add some new operation records to the event log in order to make the resulting sequence of operations correct. That is, the result of each <span class="tex-font-style-tt">getMin</span> operation is equal to the result in the record, and the heap is non-empty when <span class="tex-font-style-tt">getMin</span> ad <span class="tex-font-style-tt">removeMin</span> are applied. Vova wants to complete this as fast as possible, as the Petya may get back at any moment. He asks you to add the least possible number of operation records to the current log. Note that arbitrary number of operations may be added at the beginning, between any two other operations, or at the end of the log.</p></div><div class="input-specification"><p>The first line of the input contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of the records left in Petya's journal.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines describe the records in the current log in the order they are applied. Format described in the statement is used. All numbers in the input are integers not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span> by their absolute value.</p></div><div class="output-specification"><p>The first line of the output should contain a single integer <span class="tex-span"><i>m</i></span>&nbsp;— the minimum possible number of records in the modified sequence of operations.</p><p>Next <span class="tex-span"><i>m</i></span> lines should contain the corrected sequence of records following the format of the input (described in the statement), one per line and in the order they are applied. All the numbers in the output should be integers not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span> by their absolute value.</p><p>Note that the input sequence of operations must be the <span class="tex-font-style-bf">subsequence</span> of the output sequence.</p><p>It's guaranteed that there exists the correct answer consisting of no more than <span class="tex-span">1 000 000</span> operations.</p></div>

## Input

<p>The first line of the input contains the only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of the records left in Petya's journal.</p><p>Each of the following <span class="tex-span"><i>n</i></span> lines describe the records in the current log in the order they are applied. Format described in the statement is used. All numbers in the input are integers not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span> by their absolute value.</p>

## Output

<p>The first line of the output should contain a single integer <span class="tex-span"><i>m</i></span>&nbsp;— the minimum possible number of records in the modified sequence of operations.</p><p>Next <span class="tex-span"><i>m</i></span> lines should contain the corrected sequence of records following the format of the input (described in the statement), one per line and in the order they are applied. All the numbers in the output should be integers not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span> by their absolute value.</p><p>Note that the input sequence of operations must be the <span class="tex-font-style-bf">subsequence</span> of the output sequence.</p><p>It's guaranteed that there exists the correct answer consisting of no more than <span class="tex-span">1 000 000</span> operations.</p>





```input1
2
insert 3
getMin 4

```




```input2
4
insert 1
insert 1
removeMin
getMin 2

```




```output1
4
insert 3
removeMin
insert 4
getMin 4

```




```output2
6
insert 1
insert 1
removeMin
removeMin
insert 2
getMin 2

```



## Note

<p>In the first sample, after number <span class="tex-span">3</span> is inserted into the heap, the minimum number is <span class="tex-span">3</span>. To make the result of the first <span class="tex-font-style-tt">getMin</span> equal to <span class="tex-span">4</span> one should firstly remove number <span class="tex-span">3</span> from the heap and then add number <span class="tex-span">4</span> into the heap.</p><p>In the second sample case number <span class="tex-span">1</span> is inserted two times, so should be similarly removed twice.</p>
