## Description

<div><p>Nowadays it is becoming increasingly difficult to park a car in cities successfully. Let's imagine a segment of a street as long as <span class="tex-span"><i>L</i></span> meters along which a parking lot is located. Drivers should park their cars strictly parallel to the pavement on the right side of the street (remember that in the country the authors of the tasks come from the driving is right side!). Every driver when parking wants to leave for themselves some extra space to move their car freely, that's why a driver is looking for a place where the distance between his car and the one behind his will be no less than <span class="tex-span"><i>b</i></span> meters and the distance between his car and the one in front of his will be no less than <span class="tex-span"><i>f</i></span> meters (if there's no car behind then the car can be parked at the parking lot segment edge; the same is true for the case when there're no cars parked in front of the car). Let's introduce an axis of coordinates along the pavement. Let the parking lot begin at point 0 and end at point <span class="tex-span"><i>L</i></span>. The drivers drive in the direction of the coordinates' increasing and look for the earliest place (with the smallest possible coordinate) where they can park the car. In case there's no such place, the driver drives on searching for his perfect peaceful haven. Sometimes some cars leave the street and free some space for parking. Considering that there never are two moving cars on a street at a time write a program that can use the data on the drivers, entering the street hoping to park there and the drivers leaving it, to model the process and determine a parking lot space for each car.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>L</i></span>, <span class="tex-span"><i>b</i></span> и <span class="tex-span"><i>f</i></span> (<span class="tex-span">10 ≤ <i>L</i> ≤ 100000, 1 ≤ <i>b</i>, <i>f</i> ≤ 100</span>). The second line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) that indicates the number of requests the program has got. Every request is described on a single line and is given by two numbers. The first number represents the request type. If the request type is equal to <span class="tex-span">1</span>, then in that case the second number indicates the length of a car (in meters) that enters the street looking for a place to park. And if the request type is equal to <span class="tex-span">2</span>, then the second number identifies the number of such a request (starting with <span class="tex-span">1</span>) that the car whose arrival to the parking lot was described by a request with this number, leaves the parking lot. It is guaranteed that that car was parked at the moment the request of the <span class="tex-span">2</span> type was made. The lengths of cars are integers from <span class="tex-span">1</span> to <span class="tex-span">1000</span>.</p></div><div class="output-specification"><p>For every request of the <span class="tex-span">1</span> type print number <span class="tex-font-style-tt">-1</span> on the single line if the corresponding car couldn't find place to park along the street. Otherwise, print a single number equal to the distance between the back of the car in its parked position and the beginning of the parking lot zone.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>L</i></span>, <span class="tex-span"><i>b</i></span> и <span class="tex-span"><i>f</i></span> (<span class="tex-span">10 ≤ <i>L</i> ≤ 100000, 1 ≤ <i>b</i>, <i>f</i> ≤ 100</span>). The second line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) that indicates the number of requests the program has got. Every request is described on a single line and is given by two numbers. The first number represents the request type. If the request type is equal to <span class="tex-span">1</span>, then in that case the second number indicates the length of a car (in meters) that enters the street looking for a place to park. And if the request type is equal to <span class="tex-span">2</span>, then the second number identifies the number of such a request (starting with <span class="tex-span">1</span>) that the car whose arrival to the parking lot was described by a request with this number, leaves the parking lot. It is guaranteed that that car was parked at the moment the request of the <span class="tex-span">2</span> type was made. The lengths of cars are integers from <span class="tex-span">1</span> to <span class="tex-span">1000</span>.</p>

## Output

<p>For every request of the <span class="tex-span">1</span> type print number <span class="tex-font-style-tt">-1</span> on the single line if the corresponding car couldn't find place to park along the street. Otherwise, print a single number equal to the distance between the back of the car in its parked position and the beginning of the parking lot zone.</p>





```input1
30 1 2
6
1 5
1 4
1 5
2 2
1 5
1 4

```




```input2
30 1 1
6
1 5
1 4
1 5
2 2
1 5
1 4

```




```input3
10 1 1
1
1 12

```




```output1
0
6
11
17
23

```




```output2
0
6
11
17
6

```




```output3
-1

```


