### 声明

```C
static const char//declaration-specifiers
    (*int) a[10];//declarator (modified identifier)
```

declaration-specifiers init-declarator-list~opt~;

declaration-specifiers nonterminal:

- storage-class-specifier: `auto` `extern` `static` `register` `typedef`

- type-specifier: `void char short int long float double signed unsigned struct-or-union specifier enum-specifier typedef-name` and `their combinations`.

- type-qualifier: `const` `volatile`

declarator: identifier modified with `*` `[]` `()` which modify base type of the identifier to pointer, array or function, respectively.

