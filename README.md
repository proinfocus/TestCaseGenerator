# Test Case Generator
A tool to generate C# methods as well as test cases for those methods, quickly.

## Next Update
Working on including Exception test cases and improvements to existing Regular class where duplicate methods are added. Please watching this space for more updates.

## System Requirements
It requires .Net Framework 4.0 and above to work with no other dependencies.

## How it works?
You either type the Test case inline or create a bunch of test cases in a .txt file and pass on the file location and the tool will create all those methods on your left and test cases on your right. You could just copy them to your respective class files and take it further.

The tool aims and keeping focus on rapid development without compromising the quality of the code. Download the files and test it out today and make C# development lot quicker and better.

<b>Note:</b> The test case methods have [Fact] attributed as it was developed for <b>xunit</b>. You could just replace those with [Test] or whatever.

## Structure of the Test Case
Here is one of the sample test case:

<b>Add(1,2) = 3 => Should_Add_Two_Numbers();</b>

<b>Add(1,2) = 3</b> is the actual method you will be implementing. <b>Add(1,2)</b> is the method signature, <b> = 3</b> is the return value. This is used in the test case generation.

<b>Should_Add_Two_Numbers();</b> is the test case for the implementation.

<b> => </b> is the separator.


### Sample showing generation from Text File
![alt text](https://github.com/proinfocus/TestCaseGenerator/blob/master/screenshot-1.png)

### Sample showing generation from inline Test case
![alt text](https://github.com/proinfocus/TestCaseGenerator/blob/master/screenshot-2.png)


## Happy C# Coding!
