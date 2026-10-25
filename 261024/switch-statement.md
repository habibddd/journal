### switch statement
The switch statement is an conditional control structure that evaluates a `control expression` against a series of possible cases (`case labels`).
Each case is described by one or more statements which end should be signalled by a break statement. Without the break statement
the cases would fall through into the following one(s) until the end of the switch statement or a break or return statement is found.
```
switch (variable) {
  case 5: printf("Great\n");
          break;
  case 4: printf("Good\n");
          break;
  case 3: printf("Decent\n");
          break;
  case 2: printf("Poor\n");
          break;
  default: printf("Tough luck\n");
}
```
##### Control expression
```
switch (integer-expression) {
  ...
}
```
>[!IMPORTANT]
>```c
>switch (x)
>switch (x + 2)
>switch (grade)
>switch (character)
>```
>The control expression has to be of integer type so the examples above are all valid.
>Types such as `int`, `char`, `short`, `long`, and `enum` can therefore be used. `float`, `double`, and `strings` cannot.
##### Case label
```
case constant-integer-expression:
```
>[!IMPORTANT]
>The word *constant* is very important because it means that only a fixed integer or character is allowed. Variables, strings and floats are not valid.
>```c
>case 1:
>case 5:
>case 'A':
>case 'x':
>```
##### Statements
```
statement;
statement;
...;
break;
```
