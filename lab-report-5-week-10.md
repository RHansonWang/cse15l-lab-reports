# 2 Bugs From Lab 9
##  How you found the tests with different results (Did you use diff on the results of running a bash for loop? Did you search through manually? Did you use some other programmatic idea?)
Ans: I found the tests with different result using diff on the results of running a bash for loop stored in two files. 
## Describe which implementation is correct, or if you think neither is correct, by showing both actual outputs and indicating what the expected output is.
### Test 1: 510.md
Ans: For my implementation, The output is [/uri]. For the public one for the class, it is also outputting [/uri]. For this test, both implementations are wrong. The expected out put should be [].
### Test 2 504.md
Ans: For my implementation, The output is [/url "title", /url 'title', /url (title]. For the public one for the class, it is also outputting []. For this test, both implementations are wrong.The expected output should be [/url,/url,/url]
## For the implementation that’s not correct (or choose one if both are incorrect), describe the _bug (the problem in the code). You don’t have to provide a fix, but you should be specific about what is wrong with the program, and show the code that should be fixed.
### Test 1 : 510.md
Ans: In my implementation, the bug exists because there lacks a check for `\` before the string is added to the array \
`toReturn.add(markdown.substring(openParen + 1, closeParen));`\
The program adds in the website link no matter what is in the link, which is wrong. Could be fixed by adding a check of the string before input into array. 
### Test 2: 421.md
Ans: In my implementation, the bug exists because there lacks a check for quatation marks and useless parenthesis before the index is set to take the array \
`toReturn.add(markdown.substring(openParen + 1, closeParen));`\
The program supposes that everything in between the parenthesis is the link, it should exclude parts that should not exist in links. 