### Hi there 👋

<!--
**s26304/s26304** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

//Zadanie 1
package com.cwiczenia;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Student s1 = new Student();
        wypiszDane();
        Student s2 = new Student();
        wypiszDane();
    }
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
        + "|______________________________|");
    }
//Zadanie 2
