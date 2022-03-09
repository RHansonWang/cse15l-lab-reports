# Adding tests for MarkdownParse.java
Link to Their Repo: [https://github.com/aldrincheung/markdown-parse](https://github.com/aldrincheung/markdown-parse) 
Link to Our Repo: [https://github.com/RHansonWang/markdown-parse](https://github.com/RHansonWang/markdown-parse)
## 1. Snipplet 1
### Test: 
![image](sni1t1.png)
### My implementation:
![image](sni1tirun.png)
### Reviewed Implementation: 
![image](sni1tirun2.png)
## 2. Snipplet 2
### Test: 
![image](sni2t1.png)
### My implementation:
![image](sni2tirun.png)
### Reviewed Implementation: 
![image](sni2tirun2.png)
## 3. Snipplet 3
### Test: 
![image](sni3t1.png)
### My implementation:
![image](sni3tirun.png)
### Reviewed Implementation: 
![image](sni3tirun2.png)
## 4. Answers to question:
1. Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.\
Ans: Yes. The code should be able to fix the problem within 10 lines. By adding a check before any index is taken in, check that there isn't any backticks in between"[]", the code will exclude the links that are not correctly inputted. 

2. Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.\
Ans: Yes. I think the whole problem takes less than 10 lines to fix. It is easy to fix the nestes parentheses by basically adding an additional check on parenthesis, and take the last parenthesis before next bracket as the close index. The problem with nested brackets can be fixed by also taking the last closing bracket before parenthesis. 

3. Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.\
Ans: Yes. I think the problem can be solved within 10 lines. We could add a condition checker that checks for line breaks in link brackets. The links that contain 2 or more line breaks or line break in bracket will be excluded from result. 