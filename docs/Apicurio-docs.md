## API Designer, the Apicurito RESTful API visual designer


### Step 1: Importing APIs with Apicurio Studio


* Download the API example from [API Example](https://raw.githubusercontent.com/redhatHameed/Solution-Explorer/master/Locations.json).  and save it

* Click on Open API

* click on Edit API to walk through your newly imported API

* verify our data definitions for the API. Click on the location/phone{id} link under the Paths


 ![alt text](../images/apicurio-1.png "Create the API (service)")
 
 * Notice that this API path has a single path parameter (id defined as an int32) and a single GET operation defined. Click on the GET operation, then click the location drop-down which is part of the 200 OK response



 ![alt text](../images/apicurio-2.png "API Path (service)")
 
 
 * Verify the location object Click on the </> location object link under the Data Types section. Notice that the object has a bunch of properties defined that make up the object.
 
 
 ![alt text](../images/apicurio-3.png "API Path (location)")

 

### Step 2: Generate the Fuse Project


* Generate Fuse/Camel Java project by selecting Generate button from Apicurio dashboard and select the Fuse version.  

 ![alt text](../images/apicurio-4.png "API Path (location)")


* Download and review the project files and create a new Repo on Github and push the project.

