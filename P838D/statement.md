## Description

<div><p>There is an airplane which has <span class="tex-span"><i>n</i></span> rows from front to back. There will be <span class="tex-span"><i>m</i></span> people boarding this airplane.</p><p>This airplane has an entrance at the very front and very back of the plane.</p><p>Each person has some assigned seat. It is possible for multiple people to have the same assigned seat. The people will then board the plane one by one starting with person <span class="tex-span">1</span>. Each person can independently choose either the front entrance or back entrance to enter the plane.</p><p>When a person walks into the plane, they walk directly to their assigned seat and will try to sit in it. If it is occupied, they will continue walking in the direction they walked in until they are at empty seat - they will take the earliest empty seat that they can find. If they get to the end of the row without finding a seat, they will be angry.</p><p>Find the number of ways to assign tickets to the passengers and board the plane without anyone getting angry. Two ways are different if there exists a passenger who chose a different entrance in both ways, or the assigned seat is different. Print this count modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of input will contain two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 1 000 000</span>), the number of seats, and the number of passengers, respectively.</p></div><div class="output-specification"><p>Print a single number, the number of ways, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of input will contain two integers <span class="tex-span"><i>n</i>, <i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 1 000 000</span>), the number of seats, and the number of passengers, respectively.</p>

## Output

<p>Print a single number, the number of ways, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3 3

```




```output1
128

```



## Note

<p>Here, we will denote a passenger by which seat they were assigned, and which side they came from (either "F" or "B" for front or back, respectively).</p><p>For example, one valid way is 3B, 3B, 3B (i.e. all passengers were assigned seat 3 and came from the back entrance). Another valid way would be 2F, 1B, 3F.</p><p>One invalid way would be 2B, 2B, 2B, since the third passenger would get to the front without finding a seat.</p>
