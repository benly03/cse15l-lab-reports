Design a debugging scenario, and write your report as a conversation on EdStem. It should have:

The original post from a student with a screenshot showing a symptom and a description of a guess at the bug/some sense of what the failure-inducing input is. (Don't actually make the post! Just write the content that would go in such a post)
A response from a TA asking a leading question or suggesting a command to try (To be clear, you are mimicking a TA here.)
Another screenshot/terminal output showing what information the student got from trying that, and a clear description of what the bug is.
At the end, all the information needed about the setup including:
The file & directory structure needed
The contents of each file before fixing the bug
The full command line (or lines) you ran to trigger the bug
A description of what to edit to fix the bug
You should actually set up and run the scenario from your screenshots. It should involve at least a Java file and a bash script. Describing the bug should involve reading some output at the terminal resulting from running one or more commands. Design an error that produces more interesting output than a single message about a syntax or unbound identifier error – showcase some interesting wrong behavior! Feel free to set this up by cloning and breaking some existing code like the grading script or code from class, or by designing something of your own from scratch, etc.
# Part 1 - Debugging Scenario
The issue that is being depicted in the scenario is a student struggling to understand how to implement an `if` statement in bash. The student wants to use the `if` statement to create another case where the bash script outputs a success message after grading a submission that passes all testcases. Right now the bug would be the empty score that is being returned from the student's `grade.sh` scriptThe student submits both his `TestListExamples.java` and `grade.sh` files for the TA to observe and help.

# Student: 
Hi I'm having trouble formulating the code in my bash script to include a case where the submission passes all test cases. I noticed that the JUnit does not output the amount of tests failed so my original code shown does not correctly reflect that the submission passed all tests. Right now it's showing that successes and tests are empty. If I can get help on this I would greatly appreciate it!
![Image](testcases.png)
![Image](gradescript.png)
![Image](outputone.png)

# TA: 
Hi, have you considered how you can determine if the submission passed all test cases? (Hint: Use your failures variable as a counter) Also, consider adding more testcases to your test file.

# Student:
Hi thank you for helping me! I used the failure variable as a counter like you mentioned and checked if it was not equal to 0 and formulated my output around that. I also added more test cases! 
![Image](newtestcasesfile.png)
![Image](newgradescript.png)
![Image](successoutput.png)
