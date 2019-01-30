# Address

package com.company;

public class City_Addr implements NorthAm_Addr {


// DECLARES CLASS VARIABLES 
//
  private String City;
  private  String StreetName;
  private int StreetNumber;
  private String Country;
  private String Province_State;
  private String PostalCode_ZIP;


              // paramaterized constructor that takes the index of the address object 
              
              public City_Addr (int index){

              }
              

                // public void that takes in String paramater
                // Sets variable Country to the input
                public void setCountry(String country){

                Country = country;

                }

                
                // function that returns String Country
                public String getCountry(){

                    return Country;
                }

              // void method requires String paramater
              // sets Province_state to the String paramater
                public void setProvince_State (String province){

                Province_State = province;
                
                }
                
                // String functin returns Province_State
                public String getProvince_State(){


                    return Province_State;
                }


              // void method requires String paramater
              // sets PostalCode_ZIP to the String paramater
              
                public void setPostalCode_ZIP(String postalcode){

                  PostalCode_ZIP = postalcode;

                }
          
          
              // String functin returns PostalCode_Zip
              //
                public String getPostalCode_ZIP(){

                    return PostalCode_ZIP;
                }

              
              // void method requires String paramater
              // sets City to the String paramater
              //
                public void setCity(String city){

                  City = city;

                }

              // String functin returns City
                public String getCity (){

                  return City;
                }


                //void method requires String paramater
                // sets StreetName to the String paramater
                //
                public void setStreetName(String Street){

                StreetName = Street;

                }

                // String function returns StreetName
                public String getStreetName(){

                  return StreetName;
                }


                // public method requires int parameter
                // sets StreetNumber to that int paramater
                public void setStreetNumber(int number){


                StreetNumber = number;




                }

                // function returns integer value StreetNumber
                public int getStreetNumber(){

                  return StreetNumber;
                }












}
