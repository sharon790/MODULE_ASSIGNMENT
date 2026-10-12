# MODULE_ASSIGNMENT
      I replaced the "?" with "Sep" in Month column in the worksheet ' HOSPITAL_DETAILS' and year i did not find any missing values
      I used 'Group_by' function to find the most frequently occured data and replaced the "Smoker" column of missing values with "No" and "Hospital_tier"  "City_tier"       with 'tier - 2'
      I replaced "State_ID" column of missing values with "unknown"
      Spilted into three columns using "Spilt_column" function with delimitor " ," and " . "
      Replaced the "No major surgery" with "0" and changed the data_type to 'Whole_number'
      used 'Trim' and ' clean function to clear inconsistencies
      I created a column by using formula {   if [BMI]<18.5 then "Underweight" else if[BMI] >=18.5 and[BMI] <24.9 then "Normal Weight" else if[BMI] >=25.0 and [BMI]          <29.9 then "Overweight" else  "Obesity")  }
      I created a column by using {   if [HBA1C] <5.7 then "Normal" else if [HBA1C]>=5.7 and [HBA1C] <=6.4 then "Prediabetes" else "Diabetes"   }
      I selected the three columns and merged with customized symbol "-" and changed datatype to 'Date'
      I calculated the 'AGE' {   =DATEDIF([@[Date_of_Birth]],"08-06-2023","Y")  }
      changed data type to 'Currency'
