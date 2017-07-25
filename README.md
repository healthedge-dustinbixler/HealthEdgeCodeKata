# HealthEdgeCodeKata
String Adder

The following is a TDD Kata to build a String Adder or Calculator. 


Before you start: 

- Try not to read ahead.
- Do one task at a time. The trick is to learn to work incrementally.
- Make sure you only test for correct inputs. There is no need to test for invalid inputs for this kata.


**String Adder**

1. Create a simple String calculator with a method _int Add(string numbers)_

2. The method can take 0, 1 or 2 numbers, and will return their sum (for an empty string it will return 0) for example “” or “1” or “1,2”

--------Next Steps------------

* a) Allow the Add method to handle an unknown amount of numbers

* b) Allow the Add method to handle new lines between numbers (instead of commas): the following input is ok:  “1\n2,3”  (will equal 6)
    
    --the following input is NOT ok:  “1,\n” (no need to prove it - just clarifying)

* c) Support different delimiters

  --To change a delimiter, the beginning of the string will contain a separate line that looks like this:   “//[delimiter]\n[numbers…]” for example “//;\n1;2” should return three where the default delimiter is ‘;’ .
  
  --The first line is optional. All existing scenarios should still be supported

* d) Calling Add with a negative number will throw an exception “negatives not allowed” - and the negative that was passed. If there are multiple negatives, show all of them in the exception message

* e) Numbers bigger than 1000 should be ignored, so adding 2 + 1001  = 2

* f) Delimiters can be of any length with the following format:  “//[delimiter]\n” for example: “//[***]\n1***2***3” should return 6

* g) Allow multiple delimiters like this:  “//[delim1][delim2]\n” for example “//[*][%]\n1*2%3” should return 6.
Make sure you can also handle multiple delimiters with length longer than one char
