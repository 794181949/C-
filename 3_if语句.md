## 选择
某些代码可能执行，也可能不执行


      # include <stdio.h>
      int main(void)
      {
        if (3 > 2) // 如果表达式为真，就执行内部语句
          printf("true\n");
        return 0;
      }
      

## if 的范围问题
if 只能控制一个语句，默认情况，因此第二句的表达式会被执行，虽然缩进是一样的

    if (1 > 2) // 如果表达式为真，就执行内部语句
          printf("true\n");
          printf("true\n"); // 第二行还是会被输出
          
因此解决这个问题就需要大括号：就可以控制多个语句的执行
    if (条件)
    {
      语句A;
      语句B;
    }
      
## if else:
被看做一个语句，不能在中间加入别的内容

## 问题
空语句，意思 如果在 if ();  。。 代表了后面就是空语句， if 后面的内容都会被输出
因此 if 空语句再加一个语句后 就不能加上else，不然就会出错
同时写程序需要考虑完整性和排他性


      
## switch 的使用

      int val;
      printf("plz enter your flood:\n");
      scnaf("%d",&val);
      
      switch (val){
      case 1:
            printf("1st floor\n");
            break;
      case 2:
            printf("2nd floor\n");
            break;
      default:
            printf("too large\n");
            
case 1是程序的入口，之后会从上到下全部执行，
