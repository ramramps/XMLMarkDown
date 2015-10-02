#CodeBlockUtils
---
##Constructors 
####No public constructors defined

##Methods  
|*String* **&nbsp;&nbsp;NormalizeLineBreaks(*String* text)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns the normalized string.
|  Call this method to turn all "\r\n" and "\r" occurrences in the given string into "\n". 
| **text**
|The text to be normalized




|*String* **&nbsp;&nbsp;FormatUserText(*String* inputCode)** |  stability index:1  
| ------------- | :--------------- 
| **Return Value:** Returns the formatted code with the above process.
|  Call this method to format user codes in the following ways: 1. Leading and trailing whitespaces are removed from the original string. Characters that qualify as "whitespaces" are: '\n', '\t' and ' '. 2. Multiple statements on a single line will be broken down further into multiple statements. For example, "a = 1; b = 2;" will be broken down into two lines: "a = 1;\nb = 2;" (line break denoted by the new \n character). 3. Leading whitespaces will be removed ony for the first line. This is to preserve the indentation for lines other than the first. 4. If the resulting codes do not end with a closing curly bracket '}', then a semi-colon is appended to the code. This ensures codes like "a" will result in codes becoming "a;" 
| **inputCode**
|Original code content as typed in by the user. 







##Properties  
####No public properties defined

##Events  
####No public events defined

