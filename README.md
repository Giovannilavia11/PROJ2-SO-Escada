# Proj2 - Escada

## Grupo:
- Felipe do Nascimento Fonseca - 10409389
- Giovanni Alves Lavia - 10409448

<hr>

## Código Fonte:

<br>

```c
#include<stdlib.h>
#include<stdio.h>

int main(){
    int n, c, m, s, t, ca, v;
    char a, d;
    a = '4';
    m = 1;
    s = 0;
    t = 0;
    v = 0;

    scanf("%d", &n);
    for(int i = 0; i < n; i++) {
        scanf("%d %c", &c, &d);
        if(d != a){
            if(v > 0){
                if((c - ca) > 10){
                    s += c - ca - 10;
                }
                m++;
                v--;    
            }
            if(i == 0) t = c;
            else v++;
            ca = t;
            a = d;
        }
        t = c;
    }

    int r = c + (10 * m) - s;
    printf("%d\n", r); 

    return 0;
}
```

<hr>

## Print do Resultado do programa:

<br>

![image](https://github.com/Giovannilavia11/PROJ2-SO-Escada/assets/89709011/57f0cf87-756e-4548-90d2-6a28ab98e4e9)

<hr>
