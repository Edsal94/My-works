/*Il programma stampa una matrice 3x3 generata casualmente (con interi da 1 a 100) e successivamente stampa la trasposta, dopo averla calcolata*/

#include <stdio.h>
#define N 3
#include <time.h>
#include <stdlib.h>

void inizializza(int matrice[][N]);
void stampa(int matrice[][N]);
void trasponi(int matrice[][N]);

void stampa1(int matrice[][N]);

int main () {
int matrix[N][N];

inizializza(matrix);
stampa(matrix);
trasponi(matrix);
stampa1(matrix);

return 0;
}

void inizializza(int matrix[][N]) {
srand(time(NULL));
int i,c;

for (i=0; i<N; i++){
 for(c=0; c<N; c++) {
 matrix[i][c]=(rand()%100)+1;
 }
}
return;
}

void stampa(int matrix[][N]) {
int i,c;
for (i=0; i<N; i++) {
 for (c=0; c<N; c++) {
 printf("%d\t",matrix[c][i]);
 }
printf("\n");
}
return;
}

void trasponi(int matrix[][N]) {
int i,c;
int a,b;
for(c=0; c<N; c++) {
for (i=0; i<N; i++) {
a=matrix[i][c];
b=matrix[c][i];
matrix[i][c]=b;
matrix[c][i]=a;
c++;
}
}
return;
}

void stampa1(int matrix[][N]) {
int i,c;
printf("\nLa matrice trasposta è:\n");
for(c=0; c<N; c++) {
for (i=0; i<N; i++) {
printf("%d\t",matrix[c][i]);
}
printf("\n");
}
}
