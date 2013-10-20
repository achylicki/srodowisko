# rozwiazania, drugie zajecia
zad 1
Napisac i uruchomic program w C, ktory wczytuje liczbe naturalnan
i drukuje wartosc sumy kwadratow 1 (kwadrat) + 2 (kwadrat)...+ n(kwadrat)

```c
main ()
{
  int x,n,kwadrat;
int suma=0;
    printf ("podaj liczbe\n");
    scanf("%i", &n);
    for (x=0; x<=n; x=n++){
      kwadrat=x*x;
      suma=suma+kwadrat;
    }
    printf ("wartosc sumy kwadratu wynosi %i\n",suma);
}
```
Zad 2
Napisac program obliczajacy wartosc kazdego z ponizszych wyrazen
n1=5+3*8(2-3)
n2=2%2+2*2 -2/2
n3=2*4*(5+9

```c
main (){
  int n1,n2,n3;

  n1=5+3*8 /2-3;
  n2=2%2+2*2=2/2;
  n3=2*4*(5+9/2);

  printf("wynik dzialania to %i\n %i\n %i\n", n1, n2, n3);
  }
```

zad 3
w miejsce kropek "..." wpisz kod tak,aby powstal dzialajacy program 
/* program wpisuje liczby z tablicy tabela [] w odwrotnej kolejnosci, tj.12/6/4/2/1*/

```c
int main(){
int i;
int tabela[]={1,2,4,6,12};
for(i=4;i>=0;i=i-1)
printf("%i",tabela[i]);

return 0;

}
```
zad 4
Napisac i uruchomic program w C ktory wypisuje kolejne potegi 2 nie przekraczajace 2010
a)uzywajac pliku for
b) uzywajac pliku while

```c
int main (){
  int i;
  for(i=1;i<=2010;i=i*2)
    {
      printf("%i",i);
    }i=1;
  while(i >=2010){
printf("%i", i);
  i=i*2;
}
}
```


