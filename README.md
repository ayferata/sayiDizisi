# sayiDizisi
import java.util.Scanner;
import java.util.Arrays;

public class DiziElemanSiralamasi {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        int eleman;

        System.out.print("eleman sayisini giriniz :");
        eleman = input.nextInt();
        int[] dizi = new int[eleman];

        for (int i = 0; i < dizi.length; i++) {
            System.out.print("Sayı giriniz: "+"");
            dizi[i] = input.nextInt();
        }
        for (int j = 0; j < dizi.length; j++) {
            System.out.println(j + 1 + "." + " Eleman: "+dizi[j]);
        }
        Arrays.sort(dizi);
        System.out.println("Sıralama:" + (Arrays.toString(dizi)));
    }
}
