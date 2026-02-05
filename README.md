# OOPs-LAB02-Tasks
Name:Nikhil Kumar    Roll number:25k-3105
Q1 
package LABTASK;
import java.util.Scanner;
public class task1 {
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
                System.out.println("Welcome to point of sales");
                System.out.println("Chips 50");
                System.out.println("Hand Wash 200");
                System.out.println("Canned Almonds 125");
                System.out.println("Pickle 450");
                System.out.println("Apple juice 70");
                char choice = 'y';
                String items;
                double price;
                double Subtotal=0;
                double discount ;
                double salesTax;
                double totalBeforeTax;
                double Invoicetotal;
                while(choice=='y' || choice=='Y'){
                    sc.nextLine();
                    System.out.print("Enter the items: ");
                    items = sc.nextLine();
                    System.out.print("Enter the price: ");
                    price = sc.nextDouble();
                    Subtotal+=price;
                    System.out.print("Enter the Y/y for continue Shopping otherwise N/n for exit:");
                    choice = sc.next().charAt(0);
                }
                discount = Subtotal * 0.1;
                totalBeforeTax = Subtotal - discount;
                salesTax = 0.05* totalBeforeTax;
                Invoicetotal = totalBeforeTax + salesTax;
                System.out.println("The subtotal is:"+Subtotal);
                System.out.println("The Discount percent is:"+"10");
                System.out.println("The Discount amount is:"+discount);
                System.out.println("The total amount before tax is:"+totalBeforeTax);
                System.out.println("The Sale tax is:"+salesTax);
                System.out.println("The Invoicetotal is:"+Invoicetotal);

            }
        }


