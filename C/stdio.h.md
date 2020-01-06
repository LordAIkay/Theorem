### int getchar(void);
    single character, stdin, ASCII

    Assigning its value to a char variable will disable EOF.

### int scanf(const char *fomat, ...);
    scanf() 遇到空白符 `'\0', ' ', '\n'` 会把空白符读入然后丢弃

### char* gets(char* s)
    once gets get a `'\n'`, it read and discard it.
    
#### char* fgets(char *string, int length, FILE * stream);
    fgets() storages the `'\n'` as the last character before `'\0'`
