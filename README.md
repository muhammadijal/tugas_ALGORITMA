#include<stdio.h>

main (){

int a[2][5]={4,5,8,1,2,3,11,23,10,7};
int x=3, i, j, m, n, in, t, k, l;

    printf("Nama    : muhammad_rizal \n");
    printf("NIM     : 314 3111 016\n");
    printf("Prodi   : Manajemen Informatika  \n");
    for(i=0; i<2;i++) {
        for(j=0;j<5;j++) {
            if(a[i][j] == x) {
                printf("\nangka %d pada index ke a[%d][%d]", x, i, j);
        }
        }
    }


    printf("\n\nPengurutan Selection Sort Minimal");
    for(i=0;i<2*5-1;i++) {
        m=a[i/5][i%5];
        in=i;
        for(j=1;j<2*5-i;j++){
          n=a[(i+j)/5][(i+j)%5];
            if(m>n){
                m=n;
                in=i+j;
            }
        }
        a[in/5][in%5]=a[i/5][i%5];
        a[i/5][i%5]=m;
    }

    printf("\nHasil pengurutan dari larik tersebut adalah\n");
    for(k=0;k<=1;k++)
        for(l=0;l<5;l++)
    printf("%d\n"," ");
}
