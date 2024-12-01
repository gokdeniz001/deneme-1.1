# deneme-1.1
c üzerine denemeler

#include <stdio.h>

int main() {
    int sayi, tersSayi = 0, kalan, orijinalSayi;

  // Kullanıcıdan bir sayı al
    printf("Bir tamsayı girin: ");
    scanf("%d", &sayi);

  orijinalSayi = sayi; // Orijinal sayıyı sakla

  // Sayının tersini al
    while (sayi != 0) {
        kalan = sayi % 10;                 // Son basamağı al
        tersSayi = tersSayi * 10 + kalan; // Ters sayıyı oluştur
        sayi /= 10;                       // Son basamağı at
    }

   // Orijinal sayı ile ters sayı aynı mı kontrol et
    if (orijinalSayi == tersSayi) {
        printf("%d bir palindrom sayıdır.\n", orijinalSayi);
    } else {
        printf("%d bir palindrom sayı değildir.\n", orijinalSayi);
    }

  return 0;
}
