# Principles for writing code
### End-user experience
Any software is judged based on what the user feels when using the software. So it’s the most important that proper context is provided to the user. End-user experience must be evaluated for every code that you write.

### Meaningful variable names
The code is what developers write, read, modify day today at work. When working in a team or individual, it is most important to maintain the code in a readable format. The basic step for this is to name the variable based on the context in which it is used. As we always strive to write meaningful variable names, our code becomes easy to understand, modify and debug when needed.

### Correctness (Dry Run)
The correctness of the program must be verified immediately after completing the code. You come up with different inputs and see how the program executes. Different test cases must be thought through before writing any code. A method of tracing the program execution for different inputs on paper is called Dry Run. Use this method to find out if there are any mistakes in the logic of the program.

### Multiple solutions
For any problem we need to come up with multiple algorithms. Based on the context in which we execute this algorithm, we can choose the best one out of these multiple solutions. For example, one algorithm uses less memory and runs faster and consumes more power. It could be used on the server. Something that uses less power and even it a bit slower in runtime, we prefer to use that in the mobile. Based on the available resources and the needed response time, we can choose the algorithm. This is called the engineering tradeoff. 

For example, an application contains a list of fewer than 10 numbers and you need to see if a number exists. For this, you should not use the binary search algorithm. Instead, it would be best if you used a linear search algorithm. With more code or complicated algorithms, the chances of introducing bugs are high. So we need to go for simple algorithms in this case. The second point is, the gain you get with binary search in this situation is nothing much. So it’s preferable to use a linear search.


### List down assumptions
Always write down assumptions before writing any new function or algorithm. This is useful for other teammates to understand the code better. Also, when the assumption becomes invalid by a new situation, you can modify the code to handle the new case.


### Optimised solution
When you solve a problem, you can start with a brute force solution. But that should be only the start, not the end. Later it would be best if you came up with an efficient solution. There is a huge difference in the amount of resources that are taken by both these solutions. When you use an inefficient method, you make large server bills. The mobile battery drains with inefficient code. So it is necessary to come up with an optimal solution whenever it’s needed. 

### No duplicate code
We must never create copies of the same code in multiple locations in the codebase. When you need the same functionality in a different place, you need to refactor the required code into a function and then use that function where ever needed. With this approach, whenever there is a bug in the code, you need to fix it in only one location.  When you create multiple copies of the same code and it has some issues. You tend to fix in one location and forget it in other locations. This will lead to seeing the same bug again and fixing it multiple times. In the process, your company loses reputation with the client that you are not doing a good job. So it’s always better to refactor the needed block of code into a function.
