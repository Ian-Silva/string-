# string-

#include <stdio.h>

int main(int argc, char **argv)
{
    char sti[80],stInversa[80];
    int i, j, tam;

    fgets(sti,80,stdin);

    for(tam=0; (sti[tam]!= '\0') && (sti[tam]!='\n') ; tam++);

    stInversa[tam] = '\0';
    for(j=tam-1, i=0; j>=0; j--, i++)
    {
        stInversa[j] = sti[i];
    }

    printf("A inversa e: %s\n", stInversa);

    return 0;
}
