# sasdad
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        System.out.println("wprowadz wielkosc stopnia wielomianu: ");
        int st = scan.nextInt() + 1;
        System.out.println("podaj mnoznik: ");
        float xz = scan.nextInt();
        System.out.println("wporwadz liczby: ");
        float[] tab = new float[st];
        for (int i = 0; i < st; i++) {
            tab[i] = scan.nextFloat();
        }
        float wynik=0;
        for (int j = 0; j < st; j++)
        {
            wynik=wynik*xz+tab[j];
            System.out.print(wynik + " ");
        }
        System.out.println(": (x-"+ xz + ")");

        //System.out.println(wynik);
    }
}
