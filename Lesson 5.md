# Lesson 5

## Basic Output Function — printf

printf 函数的第一个参数始终是字符串常量即需要在屏幕上打印出来的字符序列，需要用双引号引起来

```c
printf("Hello YuCaiH");         //Hello YuCaiH 只是字符序列，可以直接打印
printf("%d",var);               //打印 var 的值到屏幕上
                                //%d is placeholder for variable
                                //"d" means decimal (十进制)
printf("%d %d", var1, var2);
//对于每个 %d 都必须提供一个相同或不同的变量
printf("%d %d %d", var1, var2, );
//如果不提供就会出现错误
```

![示例](E:\C Programming & Data Structures\printf_d.png)

从以上示例中可以清楚知道如何在程序中使用这些占位符