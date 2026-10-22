```
while (1) {
  printf("Quante case hai visitato questa sera? \n");
  if (scanf("%d", &visits) != 1) {
    printf("Input non valido: inserisci un numero intero. \n");
    while ((check = getchar()) != '\n' && check != EOF);
  } else if (visits < 1 || visits > N) {
    printf("Input non valido: inserisci un numero compreso tra 1 e %d. \n", N);
  } else {
    break;
  }
}
```
