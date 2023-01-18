## Description

<div><p>A new Berland businessman Vitaly is going to open a household appliances' store. All he's got to do now is to hire the staff.</p><p>The store will work seven days a week, but not around the clock. Every day at least <span class="tex-span"><i>k</i></span> people must work in the store.</p><p>Berland has a law that determines the order of working days and non-working days. Namely, each employee must work for exactly <span class="tex-span"><i>n</i></span> consecutive days, then rest for exactly <span class="tex-span"><i>m</i></span> days, then work for <span class="tex-span"><i>n</i></span> more days and rest for <span class="tex-span"><i>m</i></span> more, and so on. Vitaly doesn't want to break the law. Fortunately, there is a loophole: the law comes into force on the day when the employee is hired. For example, if an employee is hired on day <span class="tex-span"><i>x</i></span>, then he should work on days <span class="tex-span">[<i>x</i>, <i>x</i> + 1, ..., <i>x</i> + <i>n</i> - 1]</span>, <span class="tex-span">[<i>x</i> + <i>m</i> + <i>n</i>, <i>x</i> + <i>m</i> + <i>n</i> + 1, ..., <i>x</i> + <i>m</i> + 2<i>n</i> - 1]</span>, and so on. Day <span class="tex-span"><i>x</i></span> can be chosen arbitrarily by Vitaly.</p><p>There is one more thing: the key to the store. Berland law prohibits making copies of keys, so there is only one key. Vitaly is planning to entrust the key to the store employees. At the same time on each day the key must be with an employee who works that day — otherwise on this day no one can get inside the store. During the day the key holder can give the key to another employee, if he also works that day. The key will handed to the first hired employee at his first working day.</p><p>Each employee has to be paid salary. Therefore, Vitaly wants to hire as few employees as possible provided that the store can operate normally on each day from <span class="tex-span">1</span> to infinity. In other words, on each day with index from <span class="tex-span">1</span> to infinity, the store must have at least <span class="tex-span"><i>k</i></span> working employees, and one of the working employees should have the key to the store.</p><p>Help Vitaly and determine the minimum required number of employees, as well as days on which they should be hired.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span"><i>n</i> ≠ 1</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>In the first line print a single integer <span class="tex-span"><i>z</i></span> — the minimum required number of employees.</p><p>In the second line print <span class="tex-span"><i>z</i></span> positive integers, separated by spaces: the <span class="tex-span"><i>i</i></span>-th integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) should represent the number of the day, on which Vitaly should hire the <span class="tex-span"><i>i</i></span>-th employee.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i> ≤ 1000</span>, <span class="tex-span"><i>n</i> ≠ 1</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 1000</span>).</p>

## Output

<p>In the first line print a single integer <span class="tex-span"><i>z</i></span> — the minimum required number of employees.</p><p>In the second line print <span class="tex-span"><i>z</i></span> positive integers, separated by spaces: the <span class="tex-span"><i>i</i></span>-th integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) should represent the number of the day, on which Vitaly should hire the <span class="tex-span"><i>i</i></span>-th employee.</p><p>If there are multiple answers, print any of them.</p>





```input1
4 3 2

```




```input2
3 3 1

```




```output1
4
1 1 4 5
```




```output2
3
1 3 5
```


