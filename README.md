#Validatrix 
####A simple lightweight form validation script
Just include the script & css and add the class `.required` to your required fields and paste the init code and that's all, just 4kb.

**[View Demo](http://develus.com/github/validatrix)**

##How to use
Add class to your required fields
    
	<input class="required" name="" />

Include the validatrix script, the script requires jQuery
   
	<script src="//code.jquery.com/jquery-1.11.2.min.js"></script>
	<!-- Validatrix -->
	<link rel="stylesheet" href="validatrix/validatrix.css">
	<script src="validatrix/validatrix.js"></script>
	<script>
	$(function(){
	   $("#submit-form").click(function(){
	     if( validatrix() ){
	       alert("Submit Form");
	       }else{
	       console.log("Some fields are required");
	     }
	   return false; //Prevent form submition
	   });
	});
	</script> 

###Custom warnings

You can edit the warning values in the file `validatrix.js`

	var warnings = {
	  text : '*This text field is required',
	  textarea: '*This textarea is required',
	  select: '*Select an option',
      radio: '*Select a radio option',
	  checkbox: '*Check one option'
	}; 

 
