# Cycling Power Zone Calculator

http://jamesriall.co.uk/cycling-power-zone-calculator/

## The Project

For keen racing cyclists, the golden standard of measuring fitness is power. Power is typically measured in the number of watts someone can produce over a given duration. Given that many races are decided on climbs, where gravity creates enormous resistance, the number of watts per kilogram of bodymass a great way of determining comparative fitness to other racers.

This tool allows users to enter their personal and training data - weight, gender and their one rep wattage max for four durations - 5 second for sprint ability, 60 seconds for short term anaerobic power, 5 minutes for VO2 max power and 60 minutes for lactate threshold (or sustained power output). Once submitted the tool will then calculate a riders watts/kilogram for each duration and display it to them as well as showing them on a table how their power compares against various race categories and even professional riders! This information is used to inform riders of their relative strengths and weaknesses, help them decide on concentrations for training and racing, allow them to plan their race season, set training and race goals and more!

More information on cycling power training can be found <a href="http://home.trainingpeaks.com/blog/article/power-training-levels">here</a>.

![ScreenShot](http://res.cloudinary.com/jamesriall/image/upload/v1469029676/power_oa7ojo.png)

## The Logic

Within the index file I created the input area for the user to enter their power numbers, gender and weight. I also created a table to display all of the numbers for each gender/race category (Emmet was an enormous time saver here to save my typing out every single cell by hand).

When the user submits their information in the HTML form the JS file uses jQuery to take that inpur and save it to corresponding variables to be used throughout the program. We then work out the riders watts/kg for the various durations and save it into another set of variables. The first use of the variables is to display their absolute w/kg figures back to them in a new div. The second use is to iterate over each row in the corresponding columns and highlight the table cell with the closest w/kg value to the users data.

The forms have an element of user validation to ensure the user has input numerical values for each required field and also clears and reruns the program each time the users submits new data without having to refresh the page.

Created in June 2017