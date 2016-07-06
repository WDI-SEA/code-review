# Code Review for Krista Calderon

## Project Repo 2

[https://kamsci-mvc.herokuapp.com/](https://kamsci-mvc.herokuapp.com/)

## Review

#### Project Purpose

The purpose of this project was to be able to compare readmissions benchmarks 
of hospitals, two at at time, or against the United States as a whole.

#### Project Organization

#### Features

* The user can easily compare their readmissions benchmarks to other 
  hospitals.
  *if the user is logged in, get the stored session info
  *get info from database dataset where the userId is equal to the session user and the name is equal to the session library info and include the info from the benchmark and hospital databases that relate
  *request info from the medicare.gov api relating to the provider id and hospital provider id
  *if there is no error and the response data code is 200, parse the data and cycle through each of the measures in the measureArray
  *cycle through each of the hospitals in the singleHospitalArray and if the measure id equals the measure from the measureArray we are cycling through, push the number of readmisisons divided by the number of discharges times 100 parseFloated to the readmPercentHospitalArr.
  *request info from the medicare.gov api
  *if there is no error and the response status is 200, parse the data and cycle through the measureArray again
  *cycle through the data from the second query and if the data measure id is equal to the meausure being cycled through and it isn't "Not Available" or "Too Few to Report" then push that info to the ratioArrayU
  * if the same data is equal to the measure id and the number of readmissions or number of discharges isn't "not available" or "too few to report", add the previous pushed data to the totalReadminsU var and add the previous pushed data to the totalDischargesU var
  *set the readminPercentbyU to the totalReadminsU/totalDischargesU times 100
  and push that number to the readmPercentHospitalArrU
  *sort and store the top and bottom values and subtract the bottom value from the top
  *if the benchmark is the United States, the rationObjAll.benchmark is equal to the  ratioTopBotU which is equal to the rationObjUSA and the readmPercentHospitalArrU is equal to the readmissionsObjAll.benchmark
  response.json = reamissionObjAll, ratioObjAll, dataset, and ratioObjUSA
  *if the benchmark is not United States, make a query to the medicare.gov api looking for the state benchmark info.
  *cycle through the measureArray again and if the measure id is equal to the meausre and it isn't "Not Available" or "Too Few to Report", push the readm_ratio to the ratioArray and if the dataArray instance id is equal to the cycled measure, add the dataArray instance of number of readmissions to the totalReadmins var and add the dataArray instance of number of discharges to the totalDischarges var
  *take the totalReadmins and divide it by the totalDischarges and multiply it by 100
  *take the lowest value subtract the highest value and set that to the ratio ObjAll.benchmark
  respondwith the json of readmissionsObjAll, ratioObjAll, dataset, and ratioObjUSA
* The user can login to see their saved comparisons.
  * When the user clicks on the login link, it triggers the modal where the user can type in their email and password.  When the user clicks the submit button, the e-mail and password get checked and if the input passes, the user is redirected to the dashboard/data page and the sucess flash message is shown, otherwise the user is redirected to the homepage and the error flash message gets shown.
* The user can delete undesired comparisons from their dashbord.
  * When the user pushes the delete button next to the dataset, it takes that id, finds that in the dataset db and deletes it sending back a flash message and redirecting to the dashboard/data page.

#### Areas of Success (Code, Organization)

* Use of highcharts
  * These make the data so easy to understand the data visually and make your site look extremely professional.

* Parials
  * I like that the modals were organized in partials.  It made the rest of the code very easy to read.

#### Areas for Improvement (Code, Organization)

* I don't think you need the if(currentUser) on the nav bar of the dashboard or data pages.
  * It looks like the only way you can get to the dashboard or data pages is if you are logged in, so you could get rid of that one statement.
* Change data link a little confusing until you use it
  * I was a little confused as a user knowing what to do to get back to the data page from the dashboard page.  My first instinct was to look for a link in the navbar but there wasn't one.  Then I saw the change data link, but thought it was going to give me a drop down menu to choose other data sets but instead took me back to the data page.  I was glad to see I could get back to my data board without having to push the back button but before ever using the site I was a little confused.  Renaming it  "Back to Data" or something might fix it?

## Additional Notes

Such a great job!  Useful app and very clean and professional!