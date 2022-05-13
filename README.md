# Taksimetre-Hesaplayan-Program

Taksimetre Programı
Java ile gidilen mesafeye (KM) göre taksimetre tutarını ekrana yazdıran programı yazın.

Taksimetre KM başına 2.20 TL tutmaktadır.
Minimum ödenecek tutar 20 TL'dir. 20 TL altında ki ücretlerde yine 20 TL alınacaktır.
Taksimetre açılış ücreti 10 TL'dir.

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        //variable
         double km, tutar, fiyat=2.2,ilkTutar = 10;
        System.out.println("Km degerini giriniz : ");

        Scanner input = new Scanner(System.in);

        km = input.nextDouble();

        tutar = km*fiyat;

        if(tutar<20){
            tutar=20;
            System.out.println("Tutarınız : " + tutar);
        } else {
            tutar = tutar+ ilkTutar;
            System.out.println("Tutarınız : " + tutar);
        }
   }
}
