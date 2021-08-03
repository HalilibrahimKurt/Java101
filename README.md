# Pratik - Not Ortalaması Hesaplayan Program

import java.util.Scanner;
public class Main {
	public static void main(String[] args) {
		Scanner scanner = new Scanner(System.in);
		System.out.print("Matematik Sınav Notu:");
		int matematik = scanner.nextInt();
		System.out.print("Fizik Sınav Notu:");
		int fizik = scanner.nextInt();
		System.out.print("Kimya Sınav Notu:");
		int kimya = scanner.nextInt();
		System.out.print("Türkçe Sınav Notu:");
		int turkce = scanner.nextInt();
		System.out.print("Tarih Sınav Notu:");
		int tarih = scanner.nextInt();
		System.out.print("Müzik Sınav Notu:");
		int muzik = scanner.nextInt();
		scanner.close();
		int ortalama = (matematik+fizik+kimya+tarih+turkce+muzik)/6;
		System.out.println("Ortalama: " + ortalama);
		boolean durum = ortalama > 60;
		System.out.println("Durum: " + (durum == true ? "Geçti" : "Kaldı"));
	}
}
