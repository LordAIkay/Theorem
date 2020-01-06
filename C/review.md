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
只能是'int'一族或者'enum'

指针不可




