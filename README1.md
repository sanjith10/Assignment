1. Synopsis:

     As I’m new to this technology, I have explored and referred many websites and tutorials to accomplish the given task along with pre requisites within the time frame.
     Here I have implemented the web application testing in Ruby (Watir) with Test/unit Framework for the given client website.

2. Installation instructions:

     I.	Download and Install stable version of RUBY( Ex: 2.x.x).

          A.	Ensure that RUBY installed or not by running the following command in command prompt (>ruby –v).

     II. Install the required Ruby gems through command prompt by executing below commands.

          A.	>gem install watir-webdriver

          B.	>gem install watir

          C.	>gem install test-unit

     III. Make sure that above gems installed or not by executing the following command through command prompt (>gem query --local).

     IV.  Download chromedriver and make sure that it is placed into Ruby Bin path Ex. C:\Ruby22- x64\bin\chromedriver.exe.

     V.  Make sure that any basic editor to write/update/view the ruby code Ex. SCITE, NOTEPAD++ or any licensed version of commercial editors like RubyMine.

     VI. Make sure that dependent config.yml file is placed on the same location where the script is available.

3. How to run:

      Run the following command to execute the test file and save the results into text file through command prompt.

          >ruby main_code.rb > out.txt (main_code.rb is script file name)
		
4. Test cases implemented:

      Here I have implemented the test scenario “User Selections and Pricing Validation” for the given client website which is “https://secure.bestprice.rankingsandreviews.com/nc/homepage”.

	     For above scenario, I have implemented the below given 4 test cases
  
          I. Ensuring that selections made propagated to the next page.

          II. Ensuring that selections made have adjusted the price displayed appropriately.

          III. Validated that selections made propagated to the dashboard page by verifying the page title.

          IV. Validated that selections made in home page are displayed on the final page. 
   
5. Test cases to be implemented:

 	   If we have much more requirement details we could implement below possible test cases such as
  
         I.	Verify the certified dealers displayed are within the given radius of the zip code.

         II.	Verify the order of the certified dealers displayed to the customer (Ex: Nearest, Best).

         III.	Validate the scenario which dealer we should display if we have different dealers present within the same given radius.

         IV.	Verify the popup box with error message is displayed or not without entering the zip code value on the home page.

         V.	Verify the error messages displayed or not by skipping the mandatory fields and entering invalid inputs on the registration page. 

6. A brief explanation of your approach in completing this exercise:

      As mentioned in the assignment, I have implemented the Ruby Watir Framework and Test/Unit class to accomplish the challenge.  

      For the given scenario I have created config.yml file for simple test data and main_code.rb file which contains actual test code.

      I have implemented simple page objects testing framework in the single test file which is implementing the actual expected work flow. For that I have developed page objects and methods for every page, method for creating different browser instances and instantiated in the main script.
      I have implemented only the given positive test scenarios with the use of Ruby object oriented concepts and watir framework facilities, for creating different page object methods for different pages, in such a way that it could handle any changes in the objects in future and method for creating different browser instances. 

7. Future enhancements:

      This simple approach is made only to automate that single workflow for that website.

      Definitely we could build a strong test automation framework based on guidelines and clear requirements which will take care of complex test data files, reporting mechanism, different page object classes, action classes and generalized methods.

8. Compromises made:

      For this scenario I have compromised on reporting mechanism since I have used Test/Unit class, input data modeling and included page object methods also in the same test file whereas we could create different page action classes if we have implemented better framework. 

