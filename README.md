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
        
    public static void wypiszDane(){
        Scanner sc = new Scanner(System.in);

        System.out.println("Podaj Imię");
        String imie = sc.nextLine();
        System.out.println("Podaj Nazwisko");
        String nazwisko = sc.nextLine();
        System.out.println("Podaj płeć (Kobieta/Mężczyzna)");
        String plec = sc.nextLine();

        String napis = "";
        if (plec.equals("Mężczyzna")) napis += "Student";
        else if (plec.equals("Kobieta")) napis += "Studentka";

        System.out.println("|¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯¯|" + '\n'
        + "|" + "                              |" + '\n'
        + "|" + napis + ": " + imie + " " + nazwisko + '\n'
        + "|" + "                              |" +'\n'
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
        
    public static void kwartałRoku(){
        Scanner sc2 = new Scanner(System.in);

        System.out.println("Podaj Miesiąc (1,2,3...)");
        String miesiąc = sc2.nextLine();
        System.out.println("Podaj Rok");
        String rok = sc2.nextLine();

        String kwartał = "";
        if (miesiąc.equals ("1")) kwartał += "I ";
        else if (miesiąc.equals("2")) kwartał += "I ";
        else if (miesiąc.equals("3")) kwartał += "I ";
        else if (miesiąc.equals("4")) kwartał += "I ";
        else if (miesiąc.equals("5")) kwartał += "II ";
        else if (miesiąc.equals("6")) kwartał += "II ";
        else if (miesiąc.equals("7")) kwartał += "II ";
        else if (miesiąc.equals("8")) kwartał += "II ";
        else if (miesiąc.equals("9")) kwartał += "III ";
        else if (miesiąc.equals("10")) kwartał += "III ";
        else if (miesiąc.equals("11")) kwartał += "III ";
        else if (miesiąc.equals("12")) kwartał += "III ";

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
        
    public static boolean czyRokPrzestepny(int rok){
        return ((rok % 4 == 0) && (rok % 100 != 0 )) || (rok % 400 == 0);}
        
    public static void wyswietl(int rok, boolean czyRokPrzystepny){
        if (czyRokPrzystepny){
            System.out.println("Rok "+ rok + " jest przestępny");} 
        else {System.out.println("Rok " + rok + " nie jest przestępny");}}}
        
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

        podsumowanie(promocja,sztuki,koszt);}
        
    public static void podsumowanie(String promocja, int sztuki, double koszt){
    
        if ((promocja.equals("Tak")) && (sztuki > 10)) {
            System.out.println(koszt / 2.0);
        } else if ((promocja.equals("Tak")) && (sztuki < 10)) {
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

        String pierwszyUtwór = tytuł1 + " " + minuty1 +":" + sekundy1;
        String drugiUtwór = tytuł2 + " " + minuty2 +":" + sekundy2;
        int czasTrwaniaMinuty = (minuty1+minuty2);
        int czasTrwaniaSekundy = (sekundy1+sekundy2);
        String czasTrwania =(czasTrwaniaMinuty + ":" + czasTrwaniaSekundy);

        if ((minuty1>minuty2) && (minuty1==minuty2) || (sekundy1>sekundy2)) {System.out.println("__________________________________" + '\n' + "Utwory:" + '\n' + "1." + drugiUtwór + '\n' + "2." + pierwszyUtwór + '\n' + "Łączny czas trwania: " + czasTrwania + '\n' + "__________________________________");}
        else if ((minuty1<minuty2) && (minuty1==minuty2) || (sekundy1<sekundy2)) {System.out.println("__________________________________" + '\n' + "Utwory:" + '\n' + "1." + pierwszyUtwór + '\n' + "2." + drugiUtwór + '\n' + "Łączny czas trwania: " + czasTrwania + '\n' + "__________________________________");}
        else if ((minuty1==minuty2) && (sekundy1==sekundy2)) {System.out.println("__________________________________" + '\n' + "Utwory:" + '\n' + "1." + pierwszyUtwór + '\n' + "2." + drugiUtwór + '\n' +  "Łączny czas trwania: " + czasTrwania + '\n' + "__________________________________");}
        }}
        
        // W jaki sposób dodać minuty z sekundami?
