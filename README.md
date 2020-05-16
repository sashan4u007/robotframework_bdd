This is the example of robot framework with bdd style with allure report. 
Please change replace drivers/chromedriver with latest driver.
This example is runing on Linux (Ubuntu - 18.04) and Version 79.0.3945.117 (Official Build) (64-bit)


1. Install virtualenv package to create virtualenv

  python3 -m pip install virtualenv

2. Create virtual environment

  python3 -m virtualenv robotframework_bdd

3. Activate virtual env

  source robotframework_bdd/bin/activate

4. Install all the requirements

  pip install -r requirements.txt

5. Run test

  robot --listener 'allure_robotframework;Testresult' --include BDD test_suite/

6. Generate Allure report

  allure generate Testresult/ -o Testreport/ --clean

7. Open allure report

  allure open Testreport
