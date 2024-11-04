# JAVA-VUCUTKITLEINDEKSIHESAPLAMA
import java.util.Scanner;
import java.util.Locale;

public class VucutKitleIndeksiHesaplama {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        scanner.useLocale(Locale.FRANCE);

        // kullanıcıdan boy ve kilo bilgilerini alıyoruz
        System.out.print("Lütfen boyunuzu (metre cinsinden ) giriniz:");
        double boy = scanner.nextDouble();

        System.out.print("Lütfen kilonuzu giriniz:");
        double kilo = scanner.nextDouble();

        // Vücut Kitle İndeksi hesaplama formülü
        double vki = kilo / (boy * boy);

        // Sonucu ekrana yazdırıyoruz
        System.out.printf("Vücut Kitle İndeksiniz: %.2f", vki);
    }
}
