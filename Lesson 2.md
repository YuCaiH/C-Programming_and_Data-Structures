# Lesson 2

## C Programming - Features & The First C Programming

不要试图把所有的学习都塞进一节课中，成功的学生通常将他们的学习时间安排在较短时间内

为了完成我们想要完成的某些任务，最好的方法可能是将一项任务划分为更小的任务，然后分别处理他们

C语言的发明者也采用了类似的方法，他们将语言定义为过程语言，这仅仅意味着将巨大的程序分成更小的程序，称为过程或函数，以便我们可以轻松地使用它们，C语言的所有内容只不过是过程或函数的集合，这是C语言的主要特征

C语言是中级语言

- ## Features of C

  1. procedural programming (过程式编程)
  2. middle level language (中级语言)
  3. popular choice for system level apps (系统级应用程序的热门选择)
  4. wide variety of built in funcations,standard libraries and header files
     (丰富的内置函数、标准库和头文件)

- ## The First C Program

  ```c
  #include <stdio.h>
  int main(){
      printf("Hello YuCaiH");
      return 0;
  }
  ```

  1. ### #include <stdio.h>

     预处理器指令

     **什么是预处理器**

     预处理器的工作是将哈希符号(#)后面的文本内容替换为实际内容

        eg. **#include <stdio.h>**   是用  **实际文件stdio.h**  替换了这一行

     **Preprocessor:**  replace text (starting with #) with the actual content

     - replace before the compilation begins (在实际编译之前完成替换处理)
     - output of preprocessing is expanded source code (预处理的输出是扩展源代码，我编写的代码是源代码，现在转换为扩展的源代码)

     **#include <stdio.h>只是请求处理器包含文件stdio.h**

     **什么是stdio.h文件**

     **stdio.h : ** standard input output file (标准输入输出文件)

     扩展名为**.h**  — 这类文件称为头文件(header file)，头文件通常由我们需要的函数的声明组成（eg. stdio.h 由 printf 和 scanf 等函数的声明组成）

  2. ### 什么是函数和变量

     **函数：**C函数是解决特定问题的一组语句组成

     **变量：**用于存储计算期间使用的值的实体

  3. ### Syntax of a Function   (函数的语法)

     ![](E:\C Programming & Data Structures\Syntax of a Function.png)

     ```c
     int main(){
         printf("Hello YuCaiH");
         return 0;
     }
     ```

     函数 main 的返回类型是 int ，这意味着 main 函数在完成所有语句后将返回一个整数值， return 0; 表示如果语句执行成功则返回整数0，并退出函数，否则，如果出现其他问题，它将返回除0之外的其他整数

     在返回类型之后必须指定函数的名称(name of function)，最好选择使用见名知意的函数名，提高可读性，但无硬性规定
     主函数是预先定义的，不能更改它的名称

     函数名称的圆括号内是参数列表，这些称谓函数的输入

     main 函数没有任何参数，但是如果需要可以添加 arcc 和 arcv

  4. ### printf( ) ;

     printf 是输出函数，函数有一个用引号括起来的参数，即输出内容
     因为 printf 是在C标准库中预定义的，所以该函数后面不用跟大括号

- ## Why Different Files

  **Header files: **  declaaration of function

  **C standard library: **  actual definitions of function

  为什么我们需要不同的文件，一个用于存储函数原型，另一个用于存储实际代码

  其背后的原因是头文件 stdio.h 仅包含函数的声明，这告诉编译器我们将在函数中使用哪些函数，预处理器只需要将这些声明和实际源代码组合起来并生成扩展源代码，另一方面C标准库由函数的实际定义组成，单独维护头文件和标准库是必要的

- ## Quick Exercise

  **Task #1: Install codeblocks **

  **Task #2: make following changes to the code one by one:**

  1. Comment out the #include <stdio.h>
  2. Remove the semicolon after printf
  3. Remove int return type from main
  4. Instead of 0 in return write any integer value you want
  5. Replace 0 with some character. Characters are usually written with single quotes. For example you may write return 'a'
  6. Remove semicolon ; after return