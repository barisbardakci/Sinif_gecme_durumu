# Sinif_gecme_durumu
Java101_9 0ile100 arasındaki notların haricindekileri ortalamaya katmayan sınıf geçme durumu programı

/* Ödev - Patika.dev
Dersler : Matematik, Fizik, Türkçe, Kimya, Müzik
Geçme Notu : 55
Eğer girilen ders notları 0 veya 100 arasında değil ise ortalamaya katılmasın.*/

import java.util.Scanner;
public class Main
{
    public static void main (String[] args) {
    int matematik, fizik, turkce, kimya, muzik, toplam=0, counter=0;
    
    Scanner input=new Scanner(System.in);
    
    System.out.print("Matematik : ");
    matematik=input.nextInt();
    
    if (matematik>=0 && matematik<=100){
        toplam+=matematik;
        counter++;
    }
    System.out.print("Fizik : ");
    fizik=input.nextInt();
    
    if (fizik>=0 && fizik<=100){
        toplam+=fizik;
        counter++;
    }
    
    System.out.print("Türkçe : ");
    turkce=input.nextInt();
    
    if (turkce>=0 && turkce<=100){
        toplam+=turkce;
        counter++;
    }
    System.out.print("Kimya : ");
    kimya=input.nextInt();
    
    if (kimya>=0 && kimya<=100){
        toplam+=kimya;
        counter++;
    }
    
    System.out.print("Müzik : ");
    muzik=input.nextInt();
    
    if (muzik>=0 && muzik<=100){
        toplam+=muzik;
        counter++;
    }
    
    double average=toplam/counter ;
    
    if (average>=55) {
        System.out.println("Tebrikler, sınıfı geçtiniz");
    }else{
        System.out.println("Üzgünüm, sınıfta kaldınız");
    }
    System.out.print("Not ortalamanız :"+average);
    
    
}
    
}
