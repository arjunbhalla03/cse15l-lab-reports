# **Lab Report 5**
---
## Part 1 - Debugging Scenario
Student Message:
Hi there! I was working on Lab 3 and I ran into an error when working on ArrayExamples.java. This was the test I ran:


![Code Image](lab-report-5-error-input.png)

This was the output I received: 

![Code Image](lab-report-5-error-output.png)

I think that there may be something wrong with my actual loop and the switching but I am not too sure. Any help would be great.

TA Response:
You should look at what values are being switched. As this function reuqires you to make the swap within the array, make sure that the swap is happening correctly. Also look for how long the loop is iterating for. The other error was because our loop was looping for the entire array. By doing so, we will end up outside the array index and will not be swapping the values correctly. To fix this, we need to set our loop to only work for the first half of our array. That way all the values are correctly swapped.

Fixed Output: 

![Code Image](lab-report-5-fixed-output.png)

There were two bugs in our code. The first bug was that the array was only swapping values one way. The other value was getting lost so we needed to make sure we were storing that value somewhere and using it to complete the swap. The other bug that was present was that the loop was iterating for the entire array. It should only loop for half of it as otherwise we will just be re-swapping values and returning the array back to its initial state.

FilePath:
![Code Image](lab-report-5-filepath.png)

Initial Code:
![Code Image](lab-report-5-wrongcode.png)


Fixed Code:
![Code Image](lab-report-5-fixedcode.png)

Bash Script being used for the input:
![Code Image](lab-report-5-bashscript.png)


## Part 2 - Reflection

In the second half of the quarter, the thing I would say I appreciated learning the most was learning how to use jdb. Using jdb makes seeing what my program is actually doing step by step. There is only so many test cases you can think of so I think just being able to see what is actually happening is very beneficial. The ability to also see what the exact values of the loal fields in our code is extremely useful and is something I will most defintely be using in the future.
