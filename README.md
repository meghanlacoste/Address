# Address

package com.company;

public class City_Addr implements NorthAm_Addr {

  private String City;
  private  String StreetName;
  private int StreetNumber;
  private String Country;
  private String Province_State;
  private String PostalCode_ZIP;



              public City_Addr (int index){




              }
              



                public void setCountry(String country){

                Country = country;

                }


                public String getCountry(){

                    return Country;
                }

                public void setProvince_State (String province){


                }

                public String getProvince_State(){


                    return Province_State;
                }

                public void setPostalCode_ZIP(String postalcode){

                  PostalCode_ZIP = postalcode;

                }

                public String getPostalCode_ZIP(){


                    return PostalCode_ZIP;
                }

                public void setCity(String city){

                  City = city;

                }


                public String getCity (){

                  return City;
                }


                public void setStreetName(String Street){

                StreetName = Street;

                }


                public String getStreetName(){

                  return StreetName;
                }



                public void setStreetNumber(int number){


                StreetNumber = number;




                }


                public int getStreetNumber(){

                  return StreetNumber;
                }












}
