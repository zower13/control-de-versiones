#include <stdio.h>

int main() {
    int x = 17;
    bool y = true;

    if (x <= 1) {
        y = false;
    }
    else {
        for (int i = 2; i <=x / 2; ++i) {
            if (x % i == 0) {
                y= false;
                break;        
            }
        }
    }

    if (y == true ) {
        printf("El número %d es primo.", x);
    }
    else {
        printf("El número %d no es primo.", x);
    }
}
