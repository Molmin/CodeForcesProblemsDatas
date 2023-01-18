## Description

<div><p>A stowaway and a controller play the following game. </p><p>The train is represented by <span class="tex-span"><i>n</i></span> wagons which are numbered with positive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from the head to the tail. The stowaway and the controller are initially in some two different wagons. Every minute the train can be in one of two conditions — moving or idle. Every minute the players move.</p><p>The controller's move is as follows. The controller has the movement direction — to the train's head or to its tail. During a move the controller moves to the neighbouring wagon correspondingly to its movement direction. If at the end of his move the controller enters the <span class="tex-span">1</span>-st or the <span class="tex-span"><i>n</i></span>-th wagon, that he changes the direction of his movement into the other one. In other words, the controller cyclically goes from the train's head to its tail and back again during all the time of a game, shifting during each move by one wagon. Note, that the controller always have exactly one possible move.</p><p>The stowaway's move depends from the state of the train. If the train is moving, then the stowaway can shift to one of neighbouring wagons or he can stay where he is without moving. If the train is at a station and is idle, then the stowaway leaves the train (i.e. he is now not present in any train wagon) and then, if it is not the terminal train station, he enters the train again into any of <span class="tex-span"><i>n</i></span> wagons (not necessarily into the one he's just left and not necessarily into the neighbouring one). If the train is idle for several minutes then each such minute the stowaway leaves the train and enters it back.</p><p>Let's determine the order of the players' moves. If at the given minute the train is moving, then first the stowaway moves and then the controller does. If at this minute the train is idle, then first the stowaway leaves the train, then the controller moves and then the stowaway enters the train.</p><p>If at some point in time the stowaway and the controller happen to be in one wagon, then the controller wins: he makes the stowaway pay fine. If after a while the stowaway reaches the terminal train station, then the stowaway wins: he simply leaves the station during his move and never returns there again.</p><p>At any moment of time the players know each other's positions. The players play in the optimal way. Specifically, if the controller wins, then the stowaway plays so as to lose as late as possible. As all the possible moves for the controller are determined uniquely, then he is considered to play optimally always. Determine the winner.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span>. They represent the number of wagons in the train, the stowaway's and the controller's initial positions correspondingly (<span class="tex-span">2 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>m</i>, <i>k</i> ≤ <i>n</i></span>, <span class="tex-span"><i>m</i> ≠ <i>k</i></span>).</p><p>The second line contains the direction in which a controller moves. "to head" means that the controller moves to the train's head and "to tail" means that the controller moves to its tail. It is guaranteed that in the direction in which the controller is moving, there is at least one wagon. Wagon <span class="tex-span">1</span> is the head, and wagon <span class="tex-span"><i>n</i></span> is the tail.</p><p>The third line has the length from <span class="tex-span">1</span> to <span class="tex-span">200</span> and consists of symbols "0" and "1". The <span class="tex-span"><i>i</i></span>-th symbol contains information about the train's state at the <span class="tex-span"><i>i</i></span>-th minute of time. "0" means that in this very minute the train moves and "1" means that the train in this very minute stands idle. The last symbol of the third line is always "1" — that's the terminal train station.</p></div><div class="output-specification"><p>If the stowaway wins, print "Stowaway" without quotes. Otherwise, print "Controller" again without quotes, then, separated by a space, print the number of a minute, at which the stowaway will be caught.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span>. They represent the number of wagons in the train, the stowaway's and the controller's initial positions correspondingly (<span class="tex-span">2 ≤ <i>n</i> ≤ 50</span>, <span class="tex-span">1 ≤ <i>m</i>, <i>k</i> ≤ <i>n</i></span>, <span class="tex-span"><i>m</i> ≠ <i>k</i></span>).</p><p>The second line contains the direction in which a controller moves. "to head" means that the controller moves to the train's head and "to tail" means that the controller moves to its tail. It is guaranteed that in the direction in which the controller is moving, there is at least one wagon. Wagon <span class="tex-span">1</span> is the head, and wagon <span class="tex-span"><i>n</i></span> is the tail.</p><p>The third line has the length from <span class="tex-span">1</span> to <span class="tex-span">200</span> and consists of symbols "0" and "1". The <span class="tex-span"><i>i</i></span>-th symbol contains information about the train's state at the <span class="tex-span"><i>i</i></span>-th minute of time. "0" means that in this very minute the train moves and "1" means that the train in this very minute stands idle. The last symbol of the third line is always "1" — that's the terminal train station.</p>

## Output

<p>If the stowaway wins, print "Stowaway" without quotes. Otherwise, print "Controller" again without quotes, then, separated by a space, print the number of a minute, at which the stowaway will be caught.</p>





```input1
5 3 2
to head
0001001

```




```input2
3 2 1
to tail
0001

```




```output1
Stowaway
```




```output2
Controller 2
```


