# Lesson 3

## Introduction to Variables

比喻：Glass = Variable
           Water = Value

变量只是指向某个内存位置的名称

注意：**Declare variable before use**  (使用前声明变量)

- ## Declaration (声明)

  announcing the properties of variable to the compiler  (向编译器宣告变量的属性)

  **properties:**  ①size of the variable
                       ②name of the variable

- ## Definition (定义)

  allocating memory to a variable  (为变量分配内存)

  **Most of the time declaration and definition will be done at the same time**

```c
int var ;
//这里变量名称（name of variable）是 var ，它具有整数数据类型（data type: how much space a variable is going to occupy in memory —— it's also depends on the machine），所以通过编写 int var; 就声明了一个变量，同时请求编译器为该变量分配内存
```

- ## Initialization  (初始化)

  ```c
  int var = 3 ;
  ```

  变量的初始化并不意味着以后不能在代码中更改变量的值（variable = vary - able）

  在初始化后修改变量的值

  ```c
  #include <stdio.h>
  
  int main(){
      int var = 3 ;      //var的初始化值为3
      var = 4 ;          //将 var 的值更改为4，但是再次为其复制时并没有写 int var ，因为内存被分配给变量一次，再次定义它意味着为同一个名称再次分配内存，这是非法的，每个变量只能定义一次，但是可以在程序中通过不同的赋值多次使用
      printf("%d",var);
      return 0;
  }
  ```

  **将变量分配给变量**

  ```c
  int var1 = 3;
  int var2;
  var2 = var1;
  printf("%d",var2);
  ```

  **在一行中将相同的值分配给不同的变量**

  ```c
  int var1, var2, var3;
  var1 = var2 = var3 =4;
  printf("%d",var1);
  printf("%d",var2);
  printf("%d",var3);
  ```

  
