
### preprocessor
```C
    #include<stdio.h>
    #define foo(x,y) #x #y
    int main(){
        printf("%d\n", sizeof(foo(s,k6789)));
        printf("%s\n", foo(s,k6789));
        return 0;
    }
```
拼接了一个字符串"sk6789\0"
