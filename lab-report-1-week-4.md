# Lab Report for Weeks 3 and 4
This page contains 3 bugs and the commits that fixed them for lab 3 and 4

## Bug Number 1
Here is the screenshot of the bug fix commit:
![Commit 1](lab4-bug1.png)
The code change fixes the bug induced by [this file](https://github.com/bcli12/markdown-parse/blob/main/image-file.md).
The output of the file from the command line was this before the bug fix:
![Output 1](lab4-output2.png)
The file contains a single image, and the symptom was that the markdown file would list the image name as a link even though it isn't a link.
The bug was that the code only checked for brackets to indicate the start of a link while not checking if the brackets were from an image.
The failure inducing input contained a image, the bug caused the program to think that the image name was a link, and
the symptom was that the name of the image was listed.

## Bug Number 2
There was another code change within the same commit that fixed another bug.
![Commit 1](lab4-bug1.png)
The code change fixes the bug induced by [this file](https://github.com/bcli12/markdown-parse/blob/main/test-file.md).
The output of the file from the command line was:
![Output 1](lab4-output2.png)
