# 2.1 实验一 数据类型、运算符与表达式
## 1.实验目的
①了解算法的概念、特性、算法在程序设计中的地位。  
②熟悉算法的表示方法  
③掌握用流程图表示一个算法。  
④能独立设计一个问题的算法，并根据该算法编出问题的程序。  
⑤掌握c语言数据类型，熟悉如何定义一个整形、字符型和实型变量，以及对他们赋值的方法，了解以上类型数据输出时所用的格式转换符。  
⑥学会使用c的有关算数运算符，以及包含这些运算符的表达式，特别是自加、自减运算符的使用。  
⑦进一步熟悉c程序的编译连接和运行的过程。
## 2.实验准备
①复习算法的概念及特性。  
②复习算法的几种表示方法。  
③复习c语言的数据类型。  
④复习各种运算符和表达式。  
⑤复习自加、自减运算符并能够熟练应用。  
⑥源程序。 
## 3.实验步骤及内容
  
### 问题1：执行如下代码会怎么样？
```
#include<stdio.h>
void main(){
printf("%c",'\007');
}
```
### 问题2：把c1、c2定义成整型变量是否可以？为什么？
```
#include<stdio.h>
void main(){
    char c1,c2;
    c1 = getchar();
    c2 = getchar();
    putchar(c1);
    putchar(c2);
}
```
### 问题3：输入程序并运行：
```
#include<stdio.h>
void main(){
    char c1,c2;
    c1 = 97;
    c2 = 98;
    printf("%c %c",c1,c2);
}
```
在此基础上，进行：  
加上`printf("%d %d",c1,c2);`运行;  
第二行改为`int c1,c2`运行;  
第三行改为`c1 = 300; c2 = 400;`运行;
### 问题4：输入程序并且运行：
```
#include<stdio.h> 
void main(){
    char c1 = 'a',c2 = 'b',c3 = 'c',c4 = '\101',c5 = '\116';
    printf("a%cb%c\tc%c\tabc\n", c1,c2,c3);
    printf("\t\b%c%c",c4,c5);
}
```
## 4.实验报告
①流程图：本实验程序没有逻辑关系。  
②源程序：上面有。  
③调试过程中出现的问题和错误：没有。  
④实验结果：  
### A1：
![image](https://github.com/studyusssssing/homework/assets/152676097/4c21b4a1-aed9-402e-9036-61e2d1e93500)  
响铃符。
### A2：
可以。char类型本质依然用数字存储。
### A3：
要求1：  
![image](https://github.com/studyusssssing/homework/assets/152676097/5df256b2-6fb9-4a8b-808c-f96a560084cc)  
要求2：  
![image](https://github.com/studyusssssing/homework/assets/152676097/5df256b2-6fb9-4a8b-808c-f96a560084cc)  
要求3：  
![image](https://github.com/studyusssssing/homework/assets/152676097/1644d59c-9272-4819-a041-7b26f938ddb4)  

### A4：
![image](https://github.com/studyusssssing/homework/assets/152676097/84d544b8-355a-4f3a-9545-53fb3cc13789)  
⑤分析原有程序和修改后的区别：仅对问题3，c1与c2超出了char类型上限。  
⑥实验感受及体会：编写程序时注意缓冲区问题。




