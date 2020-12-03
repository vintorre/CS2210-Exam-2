# CS2210-Exam-2
Exam 2

Problem 1:


1) For this problem we can break it down to what index we are visiting, at any given time we are starting at index row, column (because it is a 2D array). We know that we can only travel a maximum of 1 index away from where we started, we are always going down a row, but we can either go back in the column, stay in the same column or move up a column. We can calculate the next index from where we start, row + 1 for every row index and column +1/-1 or just coulumn, this allows us to see which move gives us the minimum path.

2) For each index in the array we will store the minimum for the next move, this way when we go through the whole array it will store the minimum paths for the whole array in row 0, this way we can just get the minimum from row 0 in order to find our answer. 

3) For this problem I decided to use IDEAL, just because it came to me when I looked at it. I used ID to go through the problem description and really figure out what you were asking us to do. After I knew what we were doing I started thinking about how I would code it (EAL), I started with storing the problems in the last row, but that would not work out because there are so many ways to get down there, so I came up with my solution of storing the minimum path to the next step in the current index, this way I can start from the bottom and work my way up, always finding the minimum path. I didn't exactly follow IDEAL exactly step by step but in some way or another I completed each step in my problem solving process. 


Problem 2:

1) For this problem we have to break up what the answer is into what is a palidrome and what isnt. The subproblems we can break it into is the single characters, this will allow us to see if the smaller strings/characters are palidromes and that way when they are put together into the bigger string we can just see if the combination of smaller strings/characters were previously palidromes and if they are then we can answer the problem to the bigger strings.

2) We can store boolean values for each of the different sub strings we can make out of a given string, this way we can just count the amount of true values to give us our final answer, since we do not have to return the string itself we can just count the amounts of trues and return that. Probably can store the answer in some sort of array.

3) I once again used IDEAL to break up this problem, I used ID to see what you wanted from the answer/ and how you got there from the input. I had to look up what a palidrome was so I could get a better understanding of what I was dealing with, after I had done that I used EAL to solve the rest of the problem and put it together in code. So I came to the conclusion that i could just store the boolean values for each substring after I saw the problem description after that I was able to break it down into code and finish the problem.


Problem 3: 

1) This problem is much like the previous problem in the sense that we can break it down into a single index subproblem. We will once again store the problem into a an array like the previous problem. The recursive/ dynamic programming aspect of this problem is we can traverse an array and as we go through it we will check the answers to previous indexes to solve the problem for the current index. So at each index we store the amount of arithmetic combinations up untill that point, this will allow us to access the answer up to that point and account for the new number at position I to solve that perticular index. So at each index we only have to account for that number at that index and see if it meets the criteria for the previous index and if it does then we add it to our arithmetic counter.

2) I stated in problem 1 we are using an array, the same size as the one given to solve for our answer. The array will hold the values of arithmetic possibilities up until that specific index, this way we could just use that array and a counter to solve for the big problem, going through and adding all of the possible combinations and returning counter at the very end. 

3) Using IDEAl I first started with breaking down the problem and analyzing the example with ID. After I knew what you were asking for I then used EA to solve the rest of the problem, I first saw that it was a lot like the previous problem, maybe even a little easier in my opinion because I am a lot more comfortable with arrays than strings so I took the same approach to this problem as I did the last. After I got a solution that I believed would work I used L to look back and trace my code to see why it worked and learn from it. 


Problem 4: 

Didnt solve


Problem 5: 

1) For this problem I used longest chain up until that point at I to solve for the next chain. I would check if the current chain we are looking at is a good contender for continuing the chain, if it is then I go into the previous chain and add the value there to 1 because my current index is a good canadite, this way I could just go through the array and see the longest chain up until each index, this way I can just return the max of the array, because each index stores the current length of the chain it is a part of. 

2) For this problem I am creating an array that is the same length as the amount of links that I have, this way I can just store the length of the chain up until that current link in the newly created array. I could also access the answer to the problem by just finding the max of my new array, because the lengths are store there and we are looking for the max. 

3) Same as before I am using IDEAL to solve this problem. I used ID to make sure I understood the problem that I was given and broke down the problem into subsections from the example. I know that I had to use dynamic programming so I broke the problem up into each index. I then used EA to code my problem, and since I am starting to understand coding dynamic problems a little easier I could tell that I had to create a new array and use my previous index to solve my current index. I then used L after I was done to trace my solution and know that I had gotten it correct. 


Problem 6:

1) Once again this problem uses a similar approach to the last problems. Once we are breaking down the integer into smaller integers we can either multiply or add the two integers together, we use another list to store the answer to the max value for each integer, so this way we can see if we should add the integer or multiply it. We use each integer as an index and we use each thing stored at that index to solve the big problem. This way at index 10 (like in the example) we should have the answer to the big problem when putting in 10 as our integer. 

2) I am going to be using an array the same size as the integer given as input. I will store the max value I could have in the index of the value I took as input. For each index in the array I am solving for the max value I could have at this point, that way I can just go back and use the previous index to solve for the current index

3) When using IDEAL I broke down the problem with ID. I used this to understand the example given and my problem statement. After I understood what I had to do I then used EA to code my problem, I knew it had to be dynamic programming so I broke the problem up into sections(mainly what I was dividing my integer up into) after I had done that I knew how to code the problem. When I was done I passed the example I was given and traced how it was pased through my algortihm using L in IDEAL. 
