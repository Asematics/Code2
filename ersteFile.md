Es ist ein wunder schöner code der berechnet ab ein jahr ein schaltjahr ist oder nicht: 

![download](https://github.com/user-attachments/assets/da45bc75-3788-44b1-ad8a-23d381d15fc2)

int istSchaltjahr(int jahr) {
    if (jahr % 400 == 0) {
        return 1; 

    }
    if (jahr % 100 == 0) {
        return 0; 
    }
    if (jahr % 4 == 0) {
        return 1; 
    }
    return 0; 
}

int main() {
    int jahr;

    
    printf("Bitte geben Sie ein Jahr ein: ");
    scanf("%d", &jahr);

    
    if (istSchaltjahr(jahr)) {
        printf("%d ist ein Schaltjahr.\n", jahr);
    } else {
        printf("%d ist kein Schaltjahr.\n", jahr);
    }

    return 0;
}
