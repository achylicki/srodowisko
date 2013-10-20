# rozwiazania, drugie zajecia
zad 1
Napisac i uruchomic program w C, ktory wczytuje liczbe naturalna n
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
n1=5+3*8/2-3
n2=2%2+2*2-2/2
n3=2*4*(5+9/2)

```c
main (){
  int n1,n2,n3;

  n1=5+3*8/2-3;
  n2=2%2+2*2-2/2;
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

#ROZWIAZANIA kolega

ZADANIE 1 - odwracanie tablicy, elementy i ilosc znane

```c

int main() {
int i
int tabela[]={1,2,4,6,12};
for(i=4,i>=0,i=i+1) printf(" %i ", tabela[i]);
return 0;
}
```

ZADANIE 2 - potegi mniejsze od 2010, petla while oraz for

```c
#include<stdio.h>
main() {

  int i;
  int potega=1;
  int granica=2010;

  for(i=1;potega<granica;i=i+1){
    printf("Potega %d stopnia = %d \n",i-1,potega);
    potega=potega*2;
  }



  potega=1;
  i=1;
  for(potega=1;potega<granica;potega=potega*2){
    printf(" %i ",potega);
  } 

  potega=1;
  while(potega<granica){
    printf(" %i ", potega);
    potega=potega*2;
    i=i+1;}


  potega=1;
  i=1;
  while(potega<granica){
    printf("Potega %d stopnia = %d \n",i-1,potega);
    potega=potega*2;
    i=i+1;
  }


}
```
ZADANIE 3 - rowzne obliczanie oraz n-ta potega dwojki

```c
main(){
  int n=66;
  int i=0;
  int iloczyn=0;
  int n1, n2,n3;
  n1=5+3*8/2-3;
  n2=2%2+2*2-2/2;
  n3=2*4*(5+9/2);
  printf("N1: %d  N2: %d  N3:  %d \n",n1,n2,n3);
  printf("Podaj N: ");
  scanf("%d",&n);
  if(n>0)  for(i=1;i<=n;i=i+1){
    iloczyn=iloczyn+i*i;
  }
  else printf("LICZBA MUSI BYC WIEKSZA od 0");
  printf("Suma iloczynow: %d ",iloczyn);
}
```
ZADANIE 4- prosi o podanie elementow tablicy (max 50). Jezeli bedzie zero, wtedy konczymy i pokazujemy w odwrotnej kolejnosci.

```c
main(){
  int i=0,liczba=1;
  int tablica[50];
  while(liczba!=0){
    printf("Podaj element numer %d :", i);
    scanf("%d",&liczba);
    tablica[i]=liczba;
    printf("Element %i = %i\n",i,liczba);
    i++;
  }
  printf("WYPISUJE!\n");
  for(i=i-2;i>=0;i--) printf(" Element %i = %i\n",i,tablica[i]);
}
```

ZADANIE 5 - zamiana na system dwojkowy
```c
#include <stdio.h>
main(){
int liczba=8;
int i;
int wynik[20];
printf("Podaj liczbę w systemie 10: ");
scanf("%i",&liczba);
i=0;
while(liczba!=0)
{
	wynik[i]=liczba%2;
	printf(" RESZTA %i przez 2 = %i ",liczba,wynik[i]);
	liczba=liczba/2;
	printf(" PO PODZIELENIU LICZBA =  %i \n", liczba);
	i++;
}
printf("\nWYNIK:");
for(i=i-1;i>=0;i--) printf(" %i ",wynik[i]);


}

```
