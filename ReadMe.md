## This package is For !

Error Handling For your Project
 
 ## Installation 
 

 ## Use
````
import { ValidateData} from 'reuseablecomponents';
```` 
````
/* In your handlechange function pass your target value and check for the type(i.e...emailID validation ,password validatation,Mobile Number Validatation,etc...) */
const handleChange =(e)=>{

    const  check = ValidateData.email(e.target.value) 
}
````