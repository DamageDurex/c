# 枚举类型
c语言中,如果想表示符号常亮而不是字面值,除了#define...外，还可以使用枚举类型
枚举类型的定义
```c
#include<stdio.h>
int main(int argc,const char **argv)
{
    enum week{ Mon=1, Tues, Wed, Thurs, Fri, Sat, Sun };
    int day;
    int * ptr_day = &day;
    scanf("%d",ptr_day);
    switch(*ptr_day){
        case Mon: puts("周一");break;
        case Tues: puts("周二");break;
        case Wed: puts("周三");break;
        case Thurs: puts("周四");break;
        case Fri: puts("周五");break;
        case Sat: puts("周六");break;
        case Sun: puts("周日");break;
        default: puts("input Error!");
    }
    return 0;	
}
```
