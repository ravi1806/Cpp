### Taking a look at a sample program

* Let’s look at a simple “hello world” program:
```cpp
  #include <iostream>
 
  int main()
  {
    std::cout << "Hello world!";
    return 0;
  }
```
* Line 1 is a special type of statement called a preprocessor directive. Preprocessor directives tell the compiler to perform a special task. In this case, we are telling the compiler that we would like to add the contents of the iostream header to our program. The iostream header allows us to access functionality from the iostream library, which will allow us to write text to the screen.
* Line 2 is blank, and is ignored by the compiler.
* Line 3 declares the main() function, which as you learned above, is mandatory. Every program must have a main() function.
* Lines 4 and 7 tell the compiler which lines are part of the main function. Everything between the opening curly brace on line 4 and the closing curly brace on line 7 is considered part of the main() function.
* Line 5 is our first statement (you can tell it’s a statement because it ends with a semicolon), and it is an output statement. std::cout is a special object that represents the console/screen. The << symbol is an operator (much like + is an operator in mathematics) called the output operator. std::cout understands that anything sent to it via the output operator should be printed on the screen. In this case, we’re sending it the text “Hello world!”.
* Line 6 is a new type of statement, called a return statement. When an executable program finishes running, the main() function sends a value back to the operating system that indicates whether it was run successfully or not.
* This particular return statement returns the value of 0 to the operating system, which means “everything went okay!”. Non-zero numbers are typically used to indicate that something went wrong, and the program had to abort
