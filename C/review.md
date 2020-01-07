### mod
a = b*q + r

a mod b = r

5.3 mod 2 is not allowed because 5.3 is a float

### ?:
wrong: a > b? b++ :return 0;

三目运算符里面必须是表达式， 不能是语句。

优先级从右到左

### a++ a--
后加a++: 返回a 的值， 并a = a + 1

前加++a: a = a + 1 并返回 变量a(非左值)

后缀自增优先级高于前缀：a+++a <=> a++ + a

### sequence point


### sizof
sizeof(float) = sizeof(short) = 4

sizeof(long long) = sizeof(double) = 8

sizeof(char) = 1

### <stdbool.h>
用true/false 需要 include 它

### switch case:
只能是`int`一族或者`enum`

指针不可

### for-loop

```C
    //这个语句成立
    for(int i = 0; i < 10; i++)
    if(i < 10){ 
    }
```

### function
if a function return adress of local variable, it will cause a warning

### static

### preprocessor
#include:

include can include all types of files

#define:

### Conditional compilation

### pointer and array
```C
    int a[10];
    printf("%p", a);
```
%p 输出 指针的值——地址
输出的是array a 的地址， 也就是说a可以当指针输出

```C
    void foo(int p[4]){
        int i = 10;
        p = &i;
        //printf("%d", p[0]);
    }
```
传进来的是指针的值——地址，原(int \*)指针不会被修改

### declaration
They are allow but will cause a warning
```C
    int **c = &c;
    int **c = &*c;
    int **c = **c;
```
Why?
```C
    int a = a;
    //a = 0;
```

### Function-calling
######`float`-type argument can be pass to a function requiring `int`-type parameter:
```C
    //The practice is right
    void func(int){}
    void main(){
        double x = 1.67;
        func(x);
    }
```

### String
###### 
```C
    //The practice is right
    void main(){
        char* x = "abcd";
        //x = "abcd";    //This practice is right
        x[2] = "a";    //This practice is wrong because 'abcd' is storages in the **Read/only Area** with codes.     
    }
```








