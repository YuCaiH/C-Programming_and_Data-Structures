# Lesson 4

## Variable Naming Conventions (变量命名约定)

**Variable name:**  composed of <u>letters</u> or combination of letters (both upercase and lowercase) and <u>digits</u>.

- ## Rule #1

  don't start variables name with digit

- ## Rule #2

  begining with underscore is valid but not recommended (以下划线开头有效，但不推荐)

  Even though an underscore counts as a letter, but don't begin variable names with an underscore.

  因为变量名数量巨大，以下划线开头的名称以解析供系统使用，在程序中使用它们可能会导致代码执行出现问题，因此最好避免使用以下划线开头的变量名

- ## Rule #3

  C language is case sensitive. Uppercase letters are different from lowercase letters

- ## Rule #4

  special characters (@, #, %, ^,&, *...) not allowed in the name of variable

- ## Rule #5

  Blanks or white spaces not allowed (不允许空格在变量名中出现)

  编译器无法将包含空格的变量名识别为单个变量，可以用下划线代替空格

- ## Rule#6

  Don't use **keywords** to name the variables

  **keywords:**  if, else, for, while, switch, int, float, long, double etc...

注：don't use loooonnnggg...names for the variables