## 定义
把一个事物所有的可能取值都列举出来

## 方法
//定义了一个数据类型，但是没有定义变量

    enum WeekDay{
      Monday, Tudesday,Wednesday, Thursday, Friday, Saturdat, Sunday
    };
    
    int main(void){
      enum WeekDay day = Wednesday;
      printf("%d\n",day); //输出结果是2， 如果在Monday = 4, 结果就是 6
      
可以配合switch 来进行数值判断从而输出内容
可以限定取值范围，让代码更安全的作用
同时让代码更直观
