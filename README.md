# Test Case Generator
A tool to generate C# methods as well as test cases for those methods, quickly.

## What's new?
Current update can now create test cases to Assert.Throw<Exception> and remove duplicate method generation in the Regular class and also defines the way you could generate it as part of the comment just above the method.

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

## For Exceptions
Here is one of the sample test case:

<b>Add(1,2) = 3,ArgumentNullException => Should_Throw_ArgumentNullException();</b>

<b>Add(1,2) = 3</b> is the actual method you will be implementing. <b>Add(1,2)</b> is the method signature, <b> = 3</b> is the return value. However <b>ArgumentNullException</b> defined in the return value, separated by <b>Comma</b>, will create the test case to <b>Assert.Throws</b> instead of <b>Assert.Equal</b>.

<b>Should_Throw_ArgumentNullException();</b> is the test case for the implementation.

<b> => </b> is the separator.

### Sample showing generation from Text File
![alt text](https://github.com/proinfocus/TestCaseGenerator/blob/master/screenshot-1.png)

### Sample showing generation from inline Test case
![alt text](https://github.com/proinfocus/TestCaseGenerator/blob/master/screenshot-2.png)


## Happy C# Coding!
