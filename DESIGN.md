   # Design

   ## 1. Input
   What does the grader take in?
   It takes in the student's written code, the BlueJ output, criteria to calculate points, an example or examples of what correct code could look like, and a list of errors in the code.

   ## 2. Output
   What does it show for each student? For the whole class?
   For each student, it shows a graded report based on the code, the BlueJ output, and the list of errors. It shows how many marks they got out of the total marks. If there are mistakes made, each mistake is numbered. It shows what the mistake was and what exactly they should do to fix it. For the whole class, it would show the most common mistake among all students.

   ## 3. How strict is it?
   If a student prints "Age:15" instead of "Age: 15", is that right or wrong? Why?
   Wrong, because the students should learn that it is necessary to be specific when giving instructions to a computer through any programming language. When they focus more on making sure their code is exactly correct, they tend to be more careful when developing more complex projects in the future.

   ## 4. What can go wrong?
   At least 5 ways student code could break the grader.
   1. There are only a certain number of mistakes that the auto-grader could identify, and those mistakes that it cannot identify will not count towards the graded report, and the marks will not be accurate. The best way for the auto-grader to be the most accurate would be to attempt to think of everything that could go wrong with a student's program and provide the auto-grader with that information.
   2. The auto-grader could be looking for code that is exactly like the example, which is especially hard for students who are beginners at Java, and might grade them down even if their code is logically correct, produces the correct output, and doesn't have any syntax errors. To fix this, the auto-grader could grade based on the criteria given and make sure that all of the student's work is fulfilled by the criteria.
   3. If the program doesn't compile, it wouldn't have all the inputs it needs to make an output, so it might get stuck and never give the graded report. To fix this, the auto-grader can only consider the part of the criteria that deals with the written code, and consider the marks for the output as 0. 
   4. Each student could give their own personalized values for variables. For example, when asked for their name, the student could provide their own name. The auto-grader might mark it incorrect, as the two values of the name variable between the student's program and the example program wouldn't match. A solution could include the auto-grader grading it based on a pattern rule, e.g. "Line 1 starts with 'Name: ' and is followed by the value of playerName".
   5. If the program never stops running, the auto-grader could never return a graded report. Solving this would require a timer for the auto-grader to wait until the output is given. For example, if there is no BlueJ output after 2 minutes since the program was run, it determines the cause of the infinite loop and it reduces points for that.

   ## 5. Test case for one real lab
   The exact output your player.java lab should print.

   Name: Ashwin
   Age: 15
   Game time: 5.8
   Special power: false

   Meet Ashwin!
   He is 15 years old.
