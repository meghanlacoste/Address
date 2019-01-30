# Address

package com.company;

import java.util.*;
import java.io.*;

public class Main {

    private static int MAX_DATA = 100;

    public static void main(String[] args) {
        

        // Initializes boolean that checks is input process is complete to false;
        Boolean done = false;
     


        // Creates an array of objects that can store up to 10 objects
        City_Addr[] addressArrays = new City_Addr[10];


        int counter = 0;

        while (!done && counter<10){


            // creates new object at the counter index 
            addressArrays[counter] = new City_Addr(counter);


            Scanner scan = new Scanner (System.in);
      

            System.out.println("Enter Country");

            String userIn  = scan.next();

            addressArrays[counter].setCountry(userIn);



            System.out.println("Enter Province");
            String userIn2 = scan.next();

            addressArrays[counter].setProvince_State(userIn2);



            System.out.println("Enter Postal Code");
            String userIn3 = scan.next();

            addressArrays[counter].setPostalCode_ZIP(userIn3);


           // Scanner scan4 = new Scanner (System.in);



            System.out.println("Enter City");
            String userIn4 = scan.next();

            addressArrays[counter].setCity(userIn4);


            System.out.println("Enter Street Number");

            int numb = scan.nextInt();

            addressArrays[counter].setStreetNumber(numb);



            System.out.println("Enter Street Name");

            String userIn5 = scan.next();

            addressArrays[counter].setStreetName(userIn5);


            // ----------------------------------------------------------------
            // after each address is entered checks with the user if they are finished.
            System.out.println("if you have entered all your data enter 'done'");

            Scanner scanner= new Scanner (System.in);
             userIn  = scanner.next();
            
            // if the scanners next input is "done" or "DONE" 
            if(userIn.equalsIgnoreCase("done") ) {


                // sets boolean done to true to break out of loop
                // Prints message to screen 
                System.out.println(" Input process finished");
                done = true;

            }


            counter +=1;

        }// end while !done


         

        // loops through all indexes n g
        for (int i = 0; i < 10; i++){

            
            if (addressArrays[i] !=null) {

                System.out.println( addressArrays[i].getCountry() + "-" + addressArrays[i].getProvince_State() + "-" +
                        addressArrays[i].getPostalCode_ZIP() + "-" +  addressArrays[i].getCity() + "-" + addressArrays[i].getStreetNumber()
                        + "-" + addressArrays[i].getStreetName());

            }



        }














    }
}
