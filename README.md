# CurrencyConvertor-21-CP-59-21-CP-77
Currency Convertor (21-CP-59, 21-CP-77)
package CurrencyConvertor;

import java.util.*;
import java.text.DecimalFormat;

public class CurrencyConvertor {

    public static void main(String[] args) {

        double amount;
        double rupee, dollar, pound, euro, yen, ringgit;
        int choice;

        DecimalFormat f = new DecimalFormat("##.##");

        Scanner sc = new Scanner(System.in);

        System.out.println("Following are the Choices:");
        System.out.println("Enter 1: Rupee");
        System.out.println("Enter 2: Dollar");
        System.out.println("Enter 3: Pound");
        System.out.println("Enter 4: Euro");
        System.out.println("Enter 5: Yen");
        System.out.println("Enter 6: Ringgit");

        System.out.print("\nChoose from above options: ");
        choice = sc.nextInt();

        System.out.println("Enter the amount you want to convert?");
        amount = sc.nextFloat();

        switch (choice) {
            case 1: // Rupee Conversion
                dollar = amount / 70;
                System.out.println(amount + " Rupee = " + f.format(dollar) + " Dollar");

                pound = amount / 88;
                System.out.println(amount + " Rupee = " + f.format(pound) + " Pound");

                euro = amount / 80;
                System.out.println(amount + " Rupee = " + f.format(euro) + " Euro");

                yen = amount / 0.63;
                System.out.println(amount + " Rupee = " + f.format(yen) + " Yen");

                ringgit = amount / 16;
                System.out.println(amount + " Rupee = " + f.format(ringgit) + " Ringgit");
                break;

            case 2: // Dollar Conversion
                rupee = amount * 70;
                System.out.println(amount + " Dollar = " + f.format(rupee) + " Rupees");

                pound = amount * 0.78;
                System.out.println(amount + " Dollar = " + f.format(pound) + " Pound");

                euro = amount * 0.87;
                System.out.println(amount + " Dollar = " + f.format(euro) + " Euro");

                yen = amount * 111.087;
                System.out.println(amount + " Dollar = " + f.format(yen) + " Yen");

                ringgit = amount * 4.17;
                System.out.println(amount + " Dollar = " + f.format(ringgit) + " Ringgit");
                break;

            case 3: // Pound Conversion
                rupee = amount * 88;
                System.out.println(amount + " Pound = " + f.format(rupee) + " Rupees");

                dollar = amount * 1.26;
                System.out.println(amount + " Pound = " + f.format(dollar) + " Dollar");

                euro = amount * 1.10;
                System.out.println(amount + " Pound = " + f.format(euro) + " Euro");

                yen = amount * 140.93;
                System.out.println(amount + " Pound = " + f.format(yen) + " Yen");

                ringgit = amount * 5.29;
                System.out.println(amount + " Pound = " + f.format(ringgit) + " Ringgit");
                break;

            case 4: // Euro Conversion
                rupee = amount * 80;
                System.out.println(amount + " Euro = " + f.format(rupee) + " Rupees");

                dollar = amount * 1.14;
                System.out.println(amount + " Euro = " + f.format(dollar) + " Dollar");

                pound = amount * 0.90;
                System.out.println(amount + " Euro = " + f.format(pound) + " Pound");

                yen = amount * 127.32;
                System.out.println(amount + " Euro = " + f.format(yen) + " Yen");

                ringgit = amount * 4.78;
                System.out.println(amount + " Euro = " + f.format(ringgit) + " Ringgit");
                break;

            case 5: // Yen Conversion
                rupee = amount * 0.63;
                System.out.println(amount + " Yen = " + f.format(rupee) + " Rupees");

                dollar = amount * 0.008;
                System.out.println(amount + " Yen = " + f.format(dollar) + " Dollar");

                pound = amount * 0.007;
                System.out.println(amount + " Yen = " + f.format(pound) + " Pound");

                euro = amount * 0.007;
                System.out.println(amount + " Yen = " + f.format(euro) + " Euro");

                ringgit = amount * 0.037;
                System.out.println(amount + " Yen = " + f.format(ringgit) + " Ringgit");
                break;

            case 6: // Ringgit Conversion
                rupee = amount * 16.8;
                System.out.println(amount + " Ringgit = " + f.format(rupee) + " Rupees");

                dollar = amount * 0.239;
                System.out.println(amount + " Ringgit = " + f.format(dollar) + " Dollar");

                pound = amount * 0.188;
                System.out.println(amount + " Ringgit = " + f.format(pound) + " Pound");

                euro = amount * 0.209;
                System.out.println(amount + " Ringgit = " + f.format(euro) + " Euro");

                yen = amount * 26.63;
                System.out.println(amount + " Ringgit = " + f.format(yen) + " Yen");
                break;

            default: // Default case
                System.out.println("Invalid Input");
        }
    }

}
