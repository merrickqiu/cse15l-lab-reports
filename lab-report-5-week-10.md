# How did I find the test cases?
I simply used ```diff``` on both ```results.txt``` files to check which tests had different results. 
I then compared the markdown files to double check that the first two differences were different bugs, which they were.

![Using Diff](diff.png)

# Test 1
My implementation is incorrect since it says that ```/foo``` is a link when the opening bracket of ```14.md``` is escaped.
The professor's implementation is correct since there are no other links in the file and it correctly recognizes ```/foo``` as not a link.

Since its not exactly a change in code but rather adding a new feature, 
the following screenshot is the code from the professor's code that I need to add to my implementation.

![Escaped characters code](escape.png)
