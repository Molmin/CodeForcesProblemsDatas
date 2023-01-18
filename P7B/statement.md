## Description

<div><p>There is little time left before the release of the first national operating system BerlOS. Some of its components are not finished yet — the memory manager is among them. According to the developers' plan, in the first release the memory manager will be very simple and rectilinear. It will support three operations: </p><ul> <li> <span class="tex-font-style-tt">alloc n</span> — to allocate <span class="tex-span"><i>n</i></span> bytes of the memory and return the allocated block's identifier <span class="tex-span"><i>x</i></span>; </li><li> <span class="tex-font-style-tt">erase x</span> — to erase the block with the identifier <span class="tex-span"><i>x</i></span>; </li><li> <span class="tex-font-style-tt">defragment</span> — to defragment the free memory, bringing all the blocks as close to the beginning of the memory as possible and preserving their respective order; </li></ul><p>The memory model in this case is very simple. It is a sequence of <span class="tex-span"><i>m</i></span> bytes, numbered for convenience from the first to the <span class="tex-span"><i>m</i></span>-th.</p><p>The first operation <span class="tex-font-style-tt">alloc n</span> takes as the only parameter the size of the memory block that is to be allocated. While processing this operation, a free block of <span class="tex-span"><i>n</i></span> successive bytes is being allocated in the memory. If the amount of such blocks is more than one, the block closest to the beginning of the memory (i.e. to the first byte) is prefered. All these bytes are marked as not free, and the memory manager returns a 32-bit integer numerical token that is the identifier of this block. If it is impossible to allocate a free block of this size, the function returns <span class="tex-font-style-tt">NULL</span>.</p><p>The second operation <span class="tex-font-style-tt">erase x</span> takes as its parameter the identifier of some block. This operation frees the system memory, marking the bytes of this block as free for further use. In the case when this identifier does not point to the previously allocated block, which has not been erased yet, the function returns <span class="tex-font-style-tt">ILLEGAL_ERASE_ARGUMENT</span>.</p><p>The last operation <span class="tex-font-style-tt">defragment</span> does not have any arguments and simply brings the occupied memory sections closer to the beginning of the memory without changing their respective order.</p><p>In the current implementation you are to use successive integers, starting with 1, as identifiers. Each successful <span class="tex-font-style-tt">alloc</span> operation procession should return following number. Unsuccessful <span class="tex-font-style-tt">alloc</span> operations do not affect numeration.</p><p>You are to write the implementation of the memory manager. You should output the returned value for each <span class="tex-font-style-tt">alloc</span> command. You should also output <span class="tex-font-style-tt">ILLEGAL_ERASE_ARGUMENT</span> for all the failed <span class="tex-font-style-tt">erase</span> commands.</p></div><div class="input-specification"><p>The first line of the input data contains two positive integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100;1 ≤ <i>m</i> ≤ 100</span>), where <span class="tex-span"><i>t</i></span> — the amount of operations given to the memory manager for processing, and <span class="tex-span"><i>m</i></span> — the available memory size in bytes. Then there follow <span class="tex-span"><i>t</i></span> lines where the operations themselves are given. The first operation is <span class="tex-font-style-tt">alloc n</span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>), where <span class="tex-span"><i>n</i></span> is an integer. The second one is <span class="tex-font-style-tt">erase x</span>, where <span class="tex-span"><i>x</i></span> is an arbitrary 32-bit integer numerical token. The third operation is <span class="tex-font-style-tt">defragment</span>. </p></div><div class="output-specification"><p>Output the sequence of lines. Each line should contain either the result of <span class="tex-font-style-tt">alloc</span> operation procession , or <span class="tex-font-style-tt">ILLEGAL_ERASE_ARGUMENT</span> as a result of failed <span class="tex-font-style-tt">erase</span> operation procession. Output lines should go in the same order in which the operations are processed. Successful procession of <span class="tex-font-style-tt">alloc</span> operation should return integers, starting with 1, as the identifiers of the allocated blocks.</p></div>

## Input

<p>The first line of the input data contains two positive integers <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100;1 ≤ <i>m</i> ≤ 100</span>), where <span class="tex-span"><i>t</i></span> — the amount of operations given to the memory manager for processing, and <span class="tex-span"><i>m</i></span> — the available memory size in bytes. Then there follow <span class="tex-span"><i>t</i></span> lines where the operations themselves are given. The first operation is <span class="tex-font-style-tt">alloc n</span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>), where <span class="tex-span"><i>n</i></span> is an integer. The second one is <span class="tex-font-style-tt">erase x</span>, where <span class="tex-span"><i>x</i></span> is an arbitrary 32-bit integer numerical token. The third operation is <span class="tex-font-style-tt">defragment</span>. </p>

## Output

<p>Output the sequence of lines. Each line should contain either the result of <span class="tex-font-style-tt">alloc</span> operation procession , or <span class="tex-font-style-tt">ILLEGAL_ERASE_ARGUMENT</span> as a result of failed <span class="tex-font-style-tt">erase</span> operation procession. Output lines should go in the same order in which the operations are processed. Successful procession of <span class="tex-font-style-tt">alloc</span> operation should return integers, starting with 1, as the identifiers of the allocated blocks.</p>





```input1
6 10
alloc 5
alloc 3
erase 1
alloc 6
defragment
alloc 6

```




```output1
1
2
NULL
3

```


