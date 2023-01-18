## Description

<div><p>Berland.Taxi is a new taxi company with <span class="tex-span"><i>k</i></span> cars which started operating in the capital of Berland just recently. The capital has <span class="tex-span"><i>n</i></span> houses on a straight line numbered from <span class="tex-span">1</span> (leftmost) to <span class="tex-span"><i>n</i></span> (rightmost), and the distance between any two neighboring houses is the same.</p><p>You have to help the company schedule all the taxi rides which come throughout the day according to the following rules: </p><ul> <li> All cars are available for picking up passengers. Initially the <span class="tex-span"><i>j</i></span>-th car is located next to the house with the number <span class="tex-span"><i>x</i><sub class="lower-index"><i>j</i></sub></span> at time <span class="tex-span">0</span>. </li><li> All cars have the same speed. It takes exactly <span class="tex-span">1</span> minute for any car to travel between neighboring houses <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span>. </li><li> The <span class="tex-span"><i>i</i></span>-th request for taxi ride comes at the time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, asking for a passenger to be picked up at the house <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and dropped off at the house <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. All requests for taxi rides are given in the increasing order of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. All <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> are distinct. </li></ul><p>When a request for taxi ride is received at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, Berland.Taxi operator assigns a car to it as follows: </p><ul> <li> Out of cars which are currently available, operator assigns the car which is the <span class="tex-font-style-it">closest</span> to the pick up spot <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Needless to say, if a car is already on a ride with a passenger, it won't be available for any rides until that passenger is dropped off at the corresponding destination. </li><li> If there are several such cars, operator will pick one of them which <span class="tex-font-style-it">has been waiting the most</span> since it became available. </li><li> If there are several such cars, operator will pick one of them which <span class="tex-font-style-it">has the lowest number</span>. </li></ul><p>After a car gets assigned to the taxi ride request: </p><ul> <li> The driver immediately starts driving from current position to the house <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> Once the car reaches house <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, the passenger is immediately picked up and the driver starts driving to house <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> Once house <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is reached, the passenger gets dropped off and the car becomes available for new rides staying next to the house <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> It is allowed for multiple cars to be located next to the same house at the same point in time, while waiting for ride requests or just passing by. </li></ul><p>If there are no available cars at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> when a request for taxi ride comes, then: </p><ul> <li> The <span class="tex-span"><i>i</i></span>-th passenger will have to wait for a car to become available. </li><li> When a car becomes available, operator will immediately assign it to this taxi ride request. </li><li> If multiple cars become available at once while the passenger is waiting, operator will pick a car out of them according to the rules described above. </li></ul><p>Operator processes taxi ride requests one by one. So if multiple passengers are waiting for the cars to become available, operator will not move on to processing the <span class="tex-span">(<i>i</i> + 1)</span>-th ride request until the car gets assigned to the <span class="tex-span"><i>i</i></span>-th ride request.</p><p>Your task is to write a program that will process the given list of <span class="tex-span"><i>m</i></span> taxi ride requests. For each request you have to find out which car will get assigned to it, and how long the passenger will have to wait for a car to arrive. Note, if there is already car located at the house <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, then the corresponding wait time will be <span class="tex-span">0</span>.</p></div><div class="input-specification"><p>The first line of input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — number of houses, number of cars, and number of taxi ride requests. The second line contains integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — initial positions of cars. <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is a house number at which the <span class="tex-span"><i>i</i></span>-th car is located initially. It's allowed for more than one car to be located next to the same house.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain information about ride requests. Each ride request is represented by integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">12</sup></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> ≠ <i>b</i><sub class="lower-index"><i>j</i></sub></span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> is time in minutes when a request is made, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> is a house where passenger needs to be picked up, and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> is a house where passenger needs to be dropped off. All taxi ride requests are given in the increasing order of <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span>. All <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> are distinct.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines: the <span class="tex-span"><i>j</i></span>-th line should contain two integer numbers, the answer for the <span class="tex-span"><i>j</i></span>-th ride request — <span class="tex-font-style-it">car number</span> assigned by the operator and <span class="tex-font-style-it">passenger wait time</span>.</p></div>

## Input

<p>The first line of input contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>k</i>, <i>m</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — number of houses, number of cars, and number of taxi ride requests. The second line contains integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) — initial positions of cars. <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> is a house number at which the <span class="tex-span"><i>i</i></span>-th car is located initially. It's allowed for more than one car to be located next to the same house.</p><p>The following <span class="tex-span"><i>m</i></span> lines contain information about ride requests. Each ride request is represented by integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">12</sup></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub> ≠ <i>b</i><sub class="lower-index"><i>j</i></sub></span>), where <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> is time in minutes when a request is made, <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span> is a house where passenger needs to be picked up, and <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> is a house where passenger needs to be dropped off. All taxi ride requests are given in the increasing order of <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span>. All <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> are distinct.</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines: the <span class="tex-span"><i>j</i></span>-th line should contain two integer numbers, the answer for the <span class="tex-span"><i>j</i></span>-th ride request — <span class="tex-font-style-it">car number</span> assigned by the operator and <span class="tex-font-style-it">passenger wait time</span>.</p>





```input1
10 1 2
3
5 2 8
9 10 3

```




```input2
5 2 1
1 5
10 3 5

```




```input3
5 2 2
1 5
10 3 5
20 4 1

```




```output1
1 1
1 5

```




```output2
1 2

```




```output3
1 2
2 1

```



## Note

<p>In the first sample test, a request comes in at time <span class="tex-span">5</span> and the car needs to get from house <span class="tex-span">3</span> to house <span class="tex-span">2</span> to pick up the passenger. Therefore wait time will be <span class="tex-span">1</span> and the ride will be completed at time <span class="tex-span">5 + 1 + 6 = 12</span>. The second request comes in at time <span class="tex-span">9</span>, so the passenger will have to wait for the car to become available at time <span class="tex-span">12</span>, and then the car needs another <span class="tex-span">2</span> minutes to get from house <span class="tex-span">8</span> to house <span class="tex-span">10</span>. So the total wait time is <span class="tex-span">3 + 2 = 5</span>. </p><p>In the second sample test, cars <span class="tex-span">1</span> and <span class="tex-span">2</span> are located at the same distance from the first passenger and have the same "wait time since it became available". Car <span class="tex-span">1</span> wins a tiebreaker according to the rules because it has the lowest number. It will come to house <span class="tex-span">3</span> at time <span class="tex-span">3</span>, so the wait time will be <span class="tex-span">2</span>.</p>
