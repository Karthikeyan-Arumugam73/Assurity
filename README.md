# Assurity Assessment Read Me

Tool used : Apache JMeter 5.5
---------

Basic Assumptions :
-----------------  Test Script is created as per the Fucntional requriements given in the email
                   Test exectuion is executed as per the Functional & Non-Functional Requirements given in the email
             

Script and Support File Uploaded in Repository:
----------------------------------------------
  Please find below the File Names & File Types
  
   1. Assurity_assessment.jmx - It is a Jmeter Script File ( Should be Place in the JMeter Bin Folder if need to execute the test)
   2. p_categoryid.csv - It is a Test data file with Category IDs ( Should be Place in the JMeter Bin Folder if need to execute the test)
   3. test_parameters.properties - It is test paramter proerties file which allow for changing ramp-up, steady state, throughput and VUser (Thread) count. ( Should be Place in the JMeter Bin Folder if need to execute the test) 
    
   4. assessment_result.jtl - It is a result file executed as lcoal test in my PC ( Can be referred for the results I executed using Aggregate Reprot Listener in JMeter)
   5. assurity_csv_file.csv - The Output file created during the test executed in my local PC ( Excuted as given in Functional Requirement Number #4 Print following values in a csv file: Category ID, Name, Path, Promotion ID, Price) - can be referred to check the output 
   
 Scripting :
 ---------
   Script was created in an Open-Source tool - Apache JMeter 5.5
   Test Assertions are written code in Groovy .
   Necessary comments are added inline in the JMeter Script file for better understanding & reference
   Filename : Assurity_assessment.jmx ( Attached in Repository)
   
   To run the script alone , follow the below instructions :
    1. Go to the JMeter bin folder from the installed Directory (Example: C:\Users\Downloads\apache-jmeter-5.5\bin)
    2. Place the Script File (Assurity_assessment.jmx) in the bin directory
    3. Place the Test Data File (p_categoryid.csv) in the bin directory
    4. Place the properties file (test_parameters.properties) in the bin directory
    5. Open the Command prompt & move to JMeter Bin directory ( Example Command: cd C:\Users\Downloads\apache-jmeter-5.5\bin)
    6. Run the following command in step 7
    7. jmeter.bat -q test_parameters.properties ( Now JMeter will open with invoking the properties file)
    8. Goto File menu and open the Script file (Assurity_assessment.jmx) which is in the JMeter bin folder
    9. Run the script by clikin the play button , you will start seeing the results in View Results Tree Listener 
   
 Performance Test Execution:
 --------------------------
    Please follow the below isntructions to run the performance test
    1. Go to the JMeter bin folder from the installed Directory (Example: C:\Users\Downloads\apache-jmeter-5.5\bin)
    2. Place the Script File (Assurity_assessment.jmx) in the bin directory
    3. Place the Test Data File (p_categoryid.csv) in the bin directory
    4. Place the properties file (test_parameters.properties) in the bin directory
    5. Open the Command prompt & move to JMeter Bin directory ( Example Command: cd C:\Users\Downloads\apache-jmeter-5.5\bin)
    6. Run the following command in step 7
    7. jmeter.bat -n -t Assurity_assessment.jmx -l assessment_result.jtl -q test_parameters.properties
    8. Once the Run compelted you will get a Message in Command window as ".. end of run"
    9. Test is successfully completed
    10. Go to the JMeter Bin folder and check for the Log file "assessment_result.jtl" which contains the results of the test executed
    11. Also check for the file name "assurity_csv_file.csv" in the same JMeter Bin folder as it containes the Output required from the test executed
    
  Performance Test Report :
  -------------------------
