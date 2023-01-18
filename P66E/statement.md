## Description

<div><p>Little Vasya's uncle is a postman. The post offices are located on one circular road. Besides, each post office has its own gas station located next to it. Petya's uncle works as follows: in the morning he should leave the house and go to some post office. In the office he receives a portion of letters and a car. Then he must drive in the given car exactly one round along the circular road and return to the starting post office (the uncle can drive along the circle in any direction, counterclockwise or clockwise). Besides, since the car belongs to the city post, it should also be fuelled with gasoline only at the Post Office stations. </p><p>The total number of stations equals to <span class="tex-span"><i>n</i></span>. One can fuel the car at the <span class="tex-span"><i>i</i></span>-th station with no more than <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> liters of gasoline. Besides, one can fuel the car no more than once at each station. Also, the distance between the <span class="tex-span">1</span>-st and the <span class="tex-span">2</span>-nd station is <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> kilometers, the distance between the <span class="tex-span">2</span>-nd and the <span class="tex-span">3</span>-rd one is <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span> kilometers, ..., between the <span class="tex-span">(<i>n</i> - 1)</span>-th and the <span class="tex-span"><i>n</i></span>-th ones the distance is <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i> - 1</sub></span> kilometers and between the <span class="tex-span"><i>n</i></span>-th and the <span class="tex-span">1</span>-st one the distance is <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i></sub></span> kilometers. Petya's uncle's high-tech car uses only one liter of gasoline per kilometer. It is known that the stations are located so that the sum of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the sum of all <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. The <span class="tex-span"><i>i</i></span>-th gas station and <span class="tex-span"><i>i</i></span>-th post office are very close, so the distance between them is <span class="tex-span">0</span> kilometers.</p><p>Thus, it becomes clear that if we start from some post offices, then it is not always possible to drive one round along a circular road. The uncle faces the following problem: to what stations can he go in the morning to be able to ride exactly one circle along the circular road and visit all the post offices that are on it?</p><p>Petya, who used to attend programming classes, has volunteered to help his uncle, but his knowledge turned out to be not enough, so he asks you to help him write the program that will solve the posed problem.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — amount of gasoline on the <span class="tex-span"><i>i</i></span>-th station. The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. They are the distances between the <span class="tex-span">1</span>-st and the <span class="tex-span">2</span>-nd gas stations, between the <span class="tex-span">2</span>-nd and the <span class="tex-span">3</span>-rd ones, ..., between the <span class="tex-span"><i>n</i></span>-th and the <span class="tex-span">1</span>-st ones, respectively. The sum of all <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals to the sum of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and is no more than <span class="tex-span">10<sup class="upper-index">9</sup></span>. Each of the numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is no less than <span class="tex-span">1</span> and no more than <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div><div class="output-specification"><p>Print on the first line the number <span class="tex-span"><i>k</i></span> — the number of possible post offices, from which the car can drive one circle along a circular road. Print on the second line <span class="tex-span"><i>k</i></span> numbers in the ascending order — the numbers of offices, from which the car can start.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — amount of gasoline on the <span class="tex-span"><i>i</i></span>-th station. The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. They are the distances between the <span class="tex-span">1</span>-st and the <span class="tex-span">2</span>-nd gas stations, between the <span class="tex-span">2</span>-nd and the <span class="tex-span">3</span>-rd ones, ..., between the <span class="tex-span"><i>n</i></span>-th and the <span class="tex-span">1</span>-st ones, respectively. The sum of all <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> equals to the sum of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and is no more than <span class="tex-span">10<sup class="upper-index">9</sup></span>. Each of the numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is no less than <span class="tex-span">1</span> and no more than <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p>

## Output

<p>Print on the first line the number <span class="tex-span"><i>k</i></span> — the number of possible post offices, from which the car can drive one circle along a circular road. Print on the second line <span class="tex-span"><i>k</i></span> numbers in the ascending order — the numbers of offices, from which the car can start.</p>





```input1
4
1 7 2 3
8 1 1 3

```




```input2
8
1 2 1 2 1 2 1 2
2 1 2 1 2 1 2 1

```




```output1
2
2 4

```




```output2
8
1 2 3 4 5 6 7 8

```


