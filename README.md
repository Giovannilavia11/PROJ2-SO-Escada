# Proj2 - Escada

## Grupo:
- Felipe do Nascimento Fonseca - 10409389
- Giovanni Alves Lavia - 10409448

<br>

## Enunciado do Projeto:

<br>

<div align="center">
    
![image](https://github.com/Giovannilavia11/PROJ2-SO-Escada/assets/89709011/037deaf1-718b-4182-aa44-baadbfed0172)

</div>

<br>

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

<br>

## Print 1 do resultado do programa:

<br>

![image](https://github.com/Giovannilavia11/PROJ2-SO-Escada/assets/89709011/00f42290-6776-4ec0-8e03-b3212ba15e48)

## Print 2 do resultado do programa:

<br>

![image](https://github.com/Giovannilavia11/PROJ2-SO-Escada/assets/89709011/4fb8a096-9cdf-418d-a6fc-36c1c4a7b35f)


## Print 3 do resultado do programa:

<br>

![image](https://github.com/Giovannilavia11/PROJ2-SO-Escada/assets/89709011/0a09d6d8-8d84-4ac4-9c9d-7aec6362dcc7)
