# Address

package com.company;

import java.util.*;
import java.io.*;

public class Main {

    private static int MAX_DATA = 100;

    public static void main(String[] args) {
        // write your code here


        Boolean done = false;
        String userIn;



        City_Addr[] addressArrays = new City_Addr[10];


        int counter = 0;

        while (!done && counter<10){

            addressArrays[counter] = new City_Addr(counter);


            Scanner scan = new Scanner (System.in);


            System.out.println("Enter Country");

            userIn  = scan.next();

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



            System.out.println("if you are done enter 'done'");

            Scanner scanner= new Scanner (System.in);
             userIn  = scanner.next();

            if(userIn.equalsIgnoreCase("done") ) {

                System.out.println("process finished");
                done = true;

            }


            counter +=1;

        }// end while !done



        for (int i = 0; i < 10; i++){

            if (addressArrays[i] !=null) {

                System.out.println( addressArrays[i].getCountry() + "-" + addressArrays[i].getProvince_State() + "-" +
                        addressArrays[i].getPostalCode_ZIP() + "-" +  addressArrays[i].getCity() + "-" + addressArrays[i].getStreetNumber()
                        + "-" + addressArrays[i].getStreetName());

            }



        }














    }
}
