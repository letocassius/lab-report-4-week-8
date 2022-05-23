# Lab report 4 week 8

## * Link to my markdown-parse repo and link to the one reviewed in week 7

* [Link to my repository](https://github.com/letocassius/markdown-parser)
* [Link to the repository reviewed](https://github.com/hsflores7/markdown-parser.git)


**Showing the code in MarkdownParseTest.java for how you turned it into a test**
<img width="896" alt="Screen Shot 2022-05-23 at 3 09 48 PM" src="https://user-images.githubusercontent.com/64039891/169913323-7fa1ef56-fe3b-4103-98cd-8afcca0cbd0a.png">

**For your implementation, the corresponding output when running the tests; if it passed, say so. If it didn’t pass, show the specific part of the JUnit output that shows the test failure.**
<img width="1068" alt="Screen Shot 2022-05-23 at 3 20 31 PM" src="https://user-images.githubusercontent.com/64039891/169914231-aeb89e4c-f03a-46b2-8032-51bf8eda6189.png">

**For the implementation you reviewed in Week 7, the corresponding output when running the tests; if it passed, say so. If it didn’t pass, show the specific part of the JUnit output that shows the test failure.**<img width="1001" alt="Screen Shot 2022-05-23 at 3 24 50 PM" src="https://user-images.githubusercontent.com/64039891/169914601-b4b12487-8b29-4563-9b72-67bd0b5f61c1.png">

## Answer the following questions with 2-3 sentences each:

* Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.

the problem is cauled when the back ticks are used. Add an if statement checks if the brackets are preceded by a backtick. We would want to ignore anything in a code block. And if not add it the link to the arraylist.

* Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.

The main problem with snippet 2 is the parantheses inside the link. It would be necessary to identify that multiple paranthesis are not the end of the link. A way to fix it is to always look for paranthesis by pairs and keep each pair in count. 

* Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.

This snippet's problem is due to an incomplete link and new lines scattered in the file. The code snippet involves newlines in brackets and parentheses, I don't think we are able to fix the problem in under 10 lines since our program is only checking for if there's a single spaces between parentheses.
