### Hi there 👋

//Zadanie 1
package com.cwiczenia;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Student s1 = new Student();
        wypiszDane();
        Student s2 = new Student();
        wypiszDane();}

    public static void wypiszDane() {
        Scanner sc = new Scanner(System.in);

        System.out.println("Podaj Imię");
        String imie = sc.nextLine();
        System.out.println("Podaj Nazwisko");
        String nazwisko = sc.nextLine();
        System.out.println("Podaj płeć (Kobieta/Mężczyzna)");
        String plec = sc.nextLine();

        String napis = "";
        if (plec.equals("Mężczyzna")) {
            napis += "Student";
        } else if (plec.equals("Kobieta")) {
            napis += "Studentka";}
        } else {
            System.out.println("Błędne dane");}    

        System.out.println("|¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯|" + '\n'
                + "|" + "                              |" + '\n'
                + "|" + napis + ": " + imie + " " + nazwisko + '\n'
                + "|" + "                              |" + '\n'
                + "|______________________________|");}}
        
//Zadanie 2
package com.cwiczenia;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Data d1 = new Data();
        kwartałRoku();
        Data d2 = new Data();
        kwartałRoku();}

    public static void kwartałRoku() {
        Scanner sc2 = new Scanner(System.in);

        System.out.println("Podaj Miesiąc (1,2,3...)");
        int miesiąc = sc2.nextInt();
        System.out.println("Podaj Rok");
        long rok = sc2.nextLong();

        String kwartał = "";
        if (miesiąc >= 1 && miesiąc <= 4) {
            kwartał += "I ";
        } else if (miesiąc >= 5 && miesiąc <= 8) {
            kwartał += "II ";
        } else if (miesiąc >= 9 && miesiąc <= 12) {
            kwartał += "III ";
        } else {
            System.out.println("Błędne dane");}

        System.out.println(miesiąc + "." + rok + " to " + kwartał + "kwartał " + rok + " roku");}}
        
//Zadanie 3    
package com.cwiczenia;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        Rok r = new Rok();

        System.out.println("Podaj Rok");
        int rok = sc.nextInt();
        czyRokPrzestepny(rok);
        wyswietl(rok, czyRokPrzestepny(rok));}

    public static boolean czyRokPrzestepny(int rok) {
        return ((rok % 4 == 0) && (rok % 100 != 0)) || (rok % 400 == 0);}

    public static void wyswietl(int rok, boolean czyRokPrzystepny) {
        if (czyRokPrzystepny == true) {
            System.out.println("Rok " + rok + " jest przestępny.");
        } else {
            System.out.println("Rok " + rok + " nie jest przestępny.");}}}
        
//Zadanie 4
package com.cwiczenia;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("Podaj ilość sztuk");
        int sztuki = sc.nextInt();
        int cena = 10;
        double koszt = sztuki * cena;

        System.out.println("Czy podane wyżej sztuki są na promocji? (Tak/Nie)");
        String promocja = sc.next();

        podsumowanie(promocja, sztuki, koszt);}

    public static void podsumowanie(String promocja, int sztuki, double koszt) {

        if (promocja.equals("Tak") && sztuki > 10) {
            System.out.println(koszt / 2.0);
        } else if (promocja.equals("Tak") && sztuki < 10) {
            System.out.println(koszt);
        } else if (promocja.equals("Nie")) {
            System.out.println(koszt + (koszt * 0.1));}}}
            
 //Zadanie 5
 package com.cwiczenia;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("Podaj tytuł pierwszego utworu:");
        String tytuł1 = sc.nextLine();
        System.out.println("Podaj czas trwania pierwszego utworu (minuty):");
        int minuty1 = sc.nextInt();
        System.out.println("Podaj czas trwania pierwszego utworu (sekundy):");
        int sekundy1 = sc.nextInt();
        System.out.println("Podaj tytuł drugiego utworu:");
        String tytuł2 = sc.next();
        System.out.println("Podaj czas trwania drugiego utworu (minuty):");
        int minuty2 = sc.nextInt();
        System.out.println("Podaj czas trwania drugiego utworu (sekundy):");
        int sekundy2 = sc.nextInt();

        String pierwszyUtwór = tytuł1 + " " + minuty1 + ":" + sekundy1;
        String drugiUtwór = tytuł2 + " " + minuty2 + ":" + sekundy2;
        double czasTrwaniaMinuty = (minuty1 + minuty2);
        double czasTrwaniaSekundy = (sekundy1 + sekundy2);
        String czasTrwania = (czasTrwaniaMinuty * 60 + ":" + czasTrwaniaSekundy);

        if ((minuty1 > minuty2) && (minuty1 == minuty2) || (sekundy1 > sekundy2)) {
            System.out.println("__________________________________" + '\n' + "Utwory:" + '\n' + "1." + drugiUtwór + '\n' + "2." + pierwszyUtwór + '\n' + "Łączny czas trwania: "             + czasTrwania + '\n' + "__________________________________");
        } else if ((minuty1 < minuty2) && (minuty1 == minuty2) || (sekundy1 < sekundy2)) {
            System.out.println("__________________________________" + '\n' + "Utwory:" + '\n' + "1." + pierwszyUtwór + '\n' + "2." + drugiUtwór + '\n' + "Łączny czas trwania: "             + czasTrwania + '\n' + "__________________________________");
        } else if ((minuty1 == minuty2) && (sekundy1 == sekundy2)) {
            System.out.println("__________________________________" + '\n' + "Utwory:" + '\n' + "1." + pierwszyUtwór + '\n' + "2." + drugiUtwór + '\n' + "Łączny czas trwania: "             + czasTrwania + '\n' + "__________________________________");}}}

        // Nadal źle się formatują minuty z sekunadami
