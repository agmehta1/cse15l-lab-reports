# Aayushi's Lab Report 2
## Three failure-inducing input's and symptoms
## 1. First Error
* Code Change: ![Image](First_error_Change.png)
* Failure Inducing Input: [TestFile2](https://github.com/agmehta1/cse15l-lab-reports/blob/main/test-file2.md)
* Symptom: ![Image](First_Error_Message.png)
* Relationship between bug, symptom and failure-inducing input: The bug was an infinite loop caused by a pair of parenthesis in a line. The file(failure-inducing-input) had these parenthesis in the middle of the brackets causing such an error. This is shown by the symptom of a java heap space error which indicates the infinite loop


## 2. Second Error
* Code Change: ![Image](SecondErrorChange.png)
* Failure Inducing Input: [TestFile3](https://github.com/agmehta1/cse15l-lab-reports/blob/main/test-file3.md)
* Symptom: ![Image](SecondErrorMessage.png)
* Relationship between bug, symptom and failure-inducing input: After editing it to fix the first error when running testfile2 we correctly get: ```[https://something.com,some-page.html]```. We now have a bug where after the first ```](``` it would start the link. The file(failure-inducing-input) has the line: ```[](][not supposed to print](https://www.icecream.com/)``` and the bug is that everything after the first ```](``` is included in the link. So the text and brackets ```][not supposed to print]``` were outputed when they shouldn't have been which was the symptom.

## 3. Third Error
* Code Change: ![Image](ThirdErrorChange.png)
* Failure Inducing Input: [TestFile8](https://github.com/agmehta1/cse15l-lab-reports/blob/main/test-file8.md)
* Symptom: ![Image](ErrorMessage3.png)
* Relationship between bug, symptom and failure-inducing input: After changing my code to fix the error from above, testfile3 now printed ```[https://www.icecream.com/]``` correctly. Now we have a bug that 
*  [](a link on the first line)
[ 
