## Description

<div><p>It is nighttime and Joe the Elusive got into the country's main bank's safe. The safe has <span class="tex-span"><i>n</i></span> cells positioned in a row, each of them contains some amount of diamonds. Let's make the problem more comfortable to work with and mark the cells with positive numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from the left to the right.</p><p>Unfortunately, Joe didn't switch the last security system off. On the plus side, he knows the way it works.</p><p>Every minute the security system calculates the total amount of diamonds for each two adjacent cells (for the cells between whose numbers difference equals <span class="tex-span">1</span>). As a result of this check we get an <span class="tex-span"><i>n</i> - 1</span> sums. If at least one of the sums differs from the corresponding sum received during the previous check, then the security system is triggered.</p><p>Joe can move the diamonds from one cell to another between the security system's checks. He manages to move them no more than <span class="tex-span"><i>m</i></span> times between two checks. One of the three following operations is regarded as moving a diamond: moving a diamond from any cell to any other one, moving a diamond from any cell to Joe's pocket, moving a diamond from Joe's pocket to any cell. Initially Joe's pocket is empty, and it can carry an unlimited amount of diamonds. It is considered that before all Joe's actions the system performs at least one check.</p><p>In the morning the bank employees will come, which is why Joe has to leave the bank before that moment. Joe has only <span class="tex-span"><i>k</i></span> minutes left before morning, and on each of these <span class="tex-span"><i>k</i></span> minutes he can perform no more than <span class="tex-span"><i>m</i></span> operations. All that remains in Joe's pocket, is considered his loot.</p><p>Calculate the largest amount of diamonds Joe can carry with him. Don't forget that the security system shouldn't be triggered (even after Joe leaves the bank) and Joe should leave before morning.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>m</i>, <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> numbers. The <span class="tex-span"><i>i</i></span>-th number is equal to the amount of diamonds in the <span class="tex-span"><i>i</i></span>-th cell — it is an integer from <span class="tex-span">0</span> to <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Print a single number — the maximum number of diamonds Joe can steal.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>, <span class="tex-span">1 ≤ <i>m</i>, <i>k</i> ≤ 10<sup class="upper-index">9</sup></span>). The next line contains <span class="tex-span"><i>n</i></span> numbers. The <span class="tex-span"><i>i</i></span>-th number is equal to the amount of diamonds in the <span class="tex-span"><i>i</i></span>-th cell — it is an integer from <span class="tex-span">0</span> to <span class="tex-span">10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Print a single number — the maximum number of diamonds Joe can steal.</p>





```input1
2 3 1
2 3

```




```input2
3 2 2
4 1 3

```




```output1
0
```




```output2
2
```



## Note

<p>In the second sample Joe can act like this:</p><p>The diamonds' initial positions are <span class="tex-span">4</span> <span class="tex-span">1</span> <span class="tex-span">3</span>.</p><p>During the first period of time Joe moves a diamond from the <span class="tex-span">1</span>-th cell to the <span class="tex-span">2</span>-th one and a diamond from the <span class="tex-span">3</span>-th cell to his pocket.</p><p>By the end of the first period the diamonds' positions are <span class="tex-span">3</span> <span class="tex-span">2</span> <span class="tex-span">2</span>. The check finds no difference and the security system doesn't go off.</p><p>During the second period Joe moves a diamond from the <span class="tex-span">3</span>-rd cell to the <span class="tex-span">2</span>-nd one and puts a diamond from the <span class="tex-span">1</span>-st cell to his pocket.</p><p>By the end of the second period the diamonds' positions are <span class="tex-span">2</span> <span class="tex-span">3</span> <span class="tex-span">1</span>. The check finds no difference again and the security system doesn't go off.</p><p>Now Joe leaves with <span class="tex-span">2</span> diamonds in his pocket.</p>
