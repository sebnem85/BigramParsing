##Create an application that can take as input any text file and output a histogram of the bigrams in the text.

###Description:

A bigram is any two adjacent words in the text. A histogram is the count of how many times that particular bigram occurred in the text. 

A well formed submission will be runnable from command line and have accompanying unit tests for the bigram parsing and counting code. You may do this in any language you wish and use any framework or data structures you wish to handle reading the files, building up the output, and running the unit tests. However the bigram parsing and counting code must be implemented by yourself.

Example:

Given the text: "The quick brown fox and the quick blue hare." The bigrams with their counts would be.

1. “the quick” 2
2. “quick brown” 1
3. “brown fox” 1
4. “fox and” 1
5. “and the” 1
6. “quick blue” 1
7. “blue hare” 1

The solution is written in C# using Dot Net Core, and using xUnit for some simple tests. It is delivered as a Console Application accepting one parameter of a file path to extract text from. Under the solution is a folder called "DemoText" that has 3 sample files. 

If running in Visual Studio, change the Debug property of the Console application to set the correct path to the test file you would like to use. If a text file is not provided as a parameter to the console application, it will use default text of the first paragraph of the Gettysburg Address.

The unit tests were written in xUnit and just passes the sample text "The quick brown fox and the quick blue hare." in from above, and count that there were 7 items returned, and that the first one had an "Occurence" value of "2"

The tests can be run from within Visual Studio or at the command prompt under the "Console.Tests" directory with the "dotnet test" command

NOTE: this is demo code, in a production app I would use dependancy injection, would pull classes and services out into their own files etc. this was built as simply as was possible while completing the excercise.
