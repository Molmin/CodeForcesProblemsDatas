## Description

<div><p>Polycarp is a regular customer at the restaurant "Ber Patio". He likes having lunches there.</p><p>"Ber Patio" has special discount program for regular customers. A customer can collect bonuses and partially cover expenses in the restaurant.</p><p>Let's assume a customer currently has <span class="tex-span"><i>b</i></span> bonuses and she has to pay <span class="tex-span"><i>r</i></span> burles for a lunch. In this case the customer can use bonuses (1 bonus = 1 burle) to reduce the payment. She can cover at most half of the payment using bonuses. However, 1 bonus will be added to the customer's bonus balance per each 10 burles she paid.</p><p>Formally:</p><ol> <li> a customer can choose any number <span class="tex-span"><i>x</i></span> of bonuses to use (<img align="middle" class="tex-formula" src="file://YjfIePve.png" style="max-width: 100.0%;max-height: 100.0%;">)), </li><li> the customer's bonus balance is reduced by <span class="tex-span"><i>x</i></span>, </li><li> the customer pays <span class="tex-span"><i>r</i> - <i>x</i></span> burles, </li><li> the customer's bonus balance is increased by <span class="tex-span">⌊(<i>r</i> - <i>x</i>) / 10⌋</span> (i.e. integer division rounded down is used). </li></ol><p>Initially, there are <span class="tex-span"><i>b</i></span> bonuses on Polycarp's account. Polycarp is going to have a lunch in "Ber Patio" for the next <span class="tex-span"><i>n</i></span> days. He estimated the values <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of burles in a receipt for the <span class="tex-span"><i>i</i></span>-th day. The sum over all receipts doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> burles.</p><p>Write a program to find the minimum number of burles Polycarp has to spend and an optimal strategy to use bonuses.</p></div><div class="input-specification"><p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">0 ≤ <i>b</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of days and initial number of bonuses Polycarp has.</p><p>The second line contains the integer sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the amount of burles in the <span class="tex-span"><i>i</i></span>-th day's receipt.</p><p>It is guaranteed that the sum of all receipts does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> burles.</p></div><div class="output-specification"><p>On the first line, print the expected minimal number of burles to pay for all <span class="tex-span"><i>n</i></span> receipts.</p><p>On the second line, print the sequence of integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number of bonuses to use on the <span class="tex-span"><i>i</i></span>-th day. If there are multiple solutions, print any of them.</p></div>

## Input

<p>The first line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">0 ≤ <i>b</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of days and initial number of bonuses Polycarp has.</p><p>The second line contains the integer sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the amount of burles in the <span class="tex-span"><i>i</i></span>-th day's receipt.</p><p>It is guaranteed that the sum of all receipts does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> burles.</p>

## Output

<p>On the first line, print the expected minimal number of burles to pay for all <span class="tex-span"><i>n</i></span> receipts.</p><p>On the second line, print the sequence of integer numbers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number of bonuses to use on the <span class="tex-span"><i>i</i></span>-th day. If there are multiple solutions, print any of them.</p>





```input1
3 21
12 75 52

```




```input2
3 39
58 64 33

```




```output1
110
2 5 22 

```




```output2
107
28 4 16 

```


