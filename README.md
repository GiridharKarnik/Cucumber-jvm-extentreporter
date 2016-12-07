# Cucumber-jvm-extentreporter
This Repository is based on sitture's [cucumber-jvm-extentreport](https://github.com/sitture/cucumber-jvm-extentreport) . Since I have migrated the project from maven to gradle I haven't forked his repo.

##Usage

Build the project in your favouring IDE or using the command prompt and include the `extendedreports.jar` file to your project and reference it either through maven or gradle.

Internally the reporter has a HashMap<String,String> object named `imageStepHashMap` which the reporter checks before writing the result of each step's result.
Whenever you need to take a screenshot push the name of the step and screenshot name to the object within the ExtentFormatter object.

`ExtentFormatter.imageStepHashMap.put(stepName,fileName);`

And please don't hesitate to contact me at giridhar.co@live.com if you face any trouble using it. 
