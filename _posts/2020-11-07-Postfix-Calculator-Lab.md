---
layout: post
title: Postfix Calculator Lab
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [ArtofData]
---


## Calculations and Average

Using a stack we were able to evaluate the value of each row: the first value was 6, second was 40, third was -162, forth was -692 and if you print the file you will be able to see all the other ones. The average of all of the final values was 6.24. 

## How is a stack used to evaluate Postfix?

In order to find the value of each row we needed to use a stack. Creating s1, I was able to seperate the operation and number. If the value was a number, I pushed it into the stack as a float. If it wasn't I popped the two most recent numbers out of the stack and then applied the respective operation. So if variables a and b were the numbers and the operation was +, I popped a and b and then created c which was a+ b outside of the stack and then I pushed the value c back into the stack. The key for this lab was that a stack is needed to seperate operations and numbers, and we have to apply the definitions - peek, push, pop - to the number or operator in the stack. Once I was able to figure out the logistic of what was going on, the coding part was a lot simpler. 

## Describe the Process 

After finishing this lab, I feel very accomplished and relieved. Since we did a homework before the previous lab that helped us with the reader I understood it better, because in this one I was pretty lost. I missed class on Monday so I struggled with how to do Postfix for a while until I asked Mr. Lee in class. Once I understood Postfix and asked a couple of questions the reasoning of using a stack became clear; I had to find a way to seperate the operations and numbers. So, I struggled for a while but learned along the way. I talked to Jake about logistics and how a stack could be used and we realized that we could use for loops and if statements to decide whether it was a operation or not. This made it a lot clearer, because then we could use pop, push and peek to manipulate the stack on whether it was an operation or not. I first incorporated the stack class at the top and then began my evaluate function. I created a stack named s1 that would help us with each row. Making the row a stack made it easier, because then we would use the "Last in First out" idea with the numbers/operators.
Transforming my reasoning into code was the hardest part. The three conditions for the computer to know it is a number is that if it is not *, +, or - so I wrote an if statement and then just that the stack would push the number as a float. This wasn't that difficult, but the other way (if it was a variable) was much more challenging. There were three cases, so I created if clauses for each one; If it was an addition, you would have to pop then then add to create c, if subtraction, pop, subtract and create c and if multiplication, pop, multiply and create c. After many trials of creating the right format and using elif or if, I finally got the correct structure. This was definitely the hardest part, and the part that I will look back on.  
Finally, we had to create an average function and incorporate it. This seemed like a breeze for me, because we already had one from last lab. I copied and pasted it, but like the last lab we had to create a new list with the final averages. I created the list at the end and the key part to know was that in my with open, we had to append each final value to the new list. Then, I wrote at the end to print the average and I got 6.24.
Overall, I learned so much - not only code, but postfix notation as well. I struggled majorly with stacks in class - especially the homework - but this lab definitely strengthened my knowledge. What went well was the actual coding after the long hours of actually understanding the lab. This was very surprising because last lab it was the opposite where I had a good idea of what to do, but coding was hard. The best feeling was seeing the long output instead of indentation errors (I had so many), and realizing that I got what I wanted.