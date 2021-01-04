## 运算符
输入运算符，功能可以通过键盘将数据输入到变量中
两个用法
1、scanf（“输入控制符”，输入参数）；键盘输入的内容转换为输入控制符所规定的格式数据然后以输入参数的值为地址的变量中

      # include <stdio.h>
      
      int main(void)
      {
        int i;
        scanf("%d", &i); // &i 代表了i的地址，&是一个取地址符号
        printf("i = %d\n",i);
        return 0;
      }
2、scanf("非输入控制符 输入控制符"); ， 必须原样输入非输入控制符

    int i, j;
    printf("plz enter two number seperated by common");
    scanf("%d,%d", &i, &j); //这里输入的时候 需要加上逗号和这里面的内容匹配，不然第二个数字就不会被输入进去
    printf("i = %d, j = %d\n", i, j);
    
    
3. 使用scanf 的时候 需要用printf来提示用户
  在时候的时候最好不要包括非输入控制符，尤其是\n
scanf对用户非法输入的处理：如果有多余的值就会在后面继续读，就需要处理 eg 123m

    int i;
    char ch;
    scanf("%d",i);
    
    while ((ch = getchar()) != '\n')
      continue;
    int j;
    scanf("%d",j);


    
    

    
