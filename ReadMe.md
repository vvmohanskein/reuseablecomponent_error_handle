## Error Handler for Your Project
This npm package provides robust error handling capabilities for your project, allowing you to easily manage and validate various types of data.
 ## Installation 
 To install the package, use the following command :
 ````
npm install reuseablecomponents
````

 ## Usage
Import the  "ValidateData" object from 'reuseablecomponents' in your project
````
import { ValidateData} from 'reuseablecomponents';
```` 
 The ValidateData object is a collection of validation functions for different types of data. Each
function takes a value `v` as input and returns an object with a `message` property indicating the
validation result. 
/* In your handlechange function pass your target value and check for the type(i.e...emailID validation ,password validatation,Mobile Number Validatation,etc...) */

## Example
````
const handleChange =(e)=>{

    const  check = ValidateData.email(e.target.value).require()
// check will have  an object In that object 
We have 2 keys  namely  requried and  message

}

````
![Code image](../assets/code.png)

## Here 
 ## Requried  
 Requried  key will throw an error if there is an Empty Field.
 ## Message  

 Regex pattern used 
   ^[^\s$&*!#^@]+@[^\s@]+\.([^\s@]{2,3})+$
Message key will throw an error  if  there is an Regex Error in the entered EmailID.
![Screenshot (20)](/assets/Screenshot%20(20).png)