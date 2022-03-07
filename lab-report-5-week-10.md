# How did I find the test cases?
I simply used ```diff``` on both ```results.txt``` files to check which tests had different results. 
I then compared the markdown files to double check that the first two differences were different bugs, which they were.

![Using Diff](diff.png)

# Test 1: 14.md
My implementation is correct since there are no other links in the file and it correctly recognizes ```/foo``` as not a link.
The professor's implementation is incorrect since it says that ```/foo``` is a link when the opening bracket of the link is escaped.

The code that finds the indexes of the brackets and parenthesis needs to also contain code to check for backslashes in the professor's code.
![Escaped characters code](escape.png)

# Test 2: 194.md
My implementation is incorrect since it thinks ```url``` is a link even with text between the brackets and the parenthesis.
The professor's implementation is correct since it recognizes ```url``` as not a link because the close bracket and parenthesis are not together.

I have code to check for this, but it is not working for some reason, so this is the code I have to fix in my implementation.
![Close bracket and parenthesis code](close.png)
