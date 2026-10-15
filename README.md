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
      I copied the 'customer_id' from the customer_data  and i typed {  =VLOOKUP(Healthcare!A2,'Customer_data'!$A:$D,3,FALSE)  } then type all the columns headings           into a new sheet "Healthcare".
      i filled the data by using formula { =VLOOKUP($A2,Medical_Examination!$A:$J,2,FALSE) } 2nd column to 10th column from "BMI till Diabetes"
      I filled the data by using formula {  =VLOOKUP($A2,Hosipital_Specialisation!$A:$K,6,FALSE) } 6th column to 11th column from "Date_of_Birth till Age"
      I inserted the pivot tables first {  column - cancer history, row - smoker, values- count of customer_Id  } then inserted dougnut chart
      I inserted the pivot tables f{  column - Sumofmajorsurgies, row - Any transplants, values- sumof major surgies and avergae of HBAIC  } then inserted PIE chart
      For healthcare charges vary by weight and diabetes status : rows- weighht_status,columns- Diabetes_status,values-average of charges
      Comparing the average charges for each hospital tier within the state : columns- Hospital_tier,  rows-State_ID,values-average of charges
      For correlation between Age and both BMI & HBA!C  - first selected both columns and inserted scatter 
      I arranged the graphs in a new sheet and inserted slicer of weight_status and Diabetes_status and connected all the pivot_tables by using report function
      
