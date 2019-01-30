package com.company;

public interface NorthAm_Addr {

   String Country = "invalid";
    String Province_State = "invalid";
     String PostalCode_ZIP = "invalid";

    void setCountry(String country);

    String getCountry();

    void setProvince_State (String province);

    String getProvince_State();

    void setPostalCode_ZIP(String postalcode);

    String getPostalCode_ZIP();




}

