# final-project-cfs.js
function idCard(){
    var firstName = document.getElementById("firstName").value;
    var lastName = document.getElementById("lastName").value;
    var address = document.getElementById("address").value;
    var age = document.getElementById("age").value;
    var phoneNumber = document.getElementById("phoneNumber").value;



    

    var numberArray = [];
    numberArray.push(age);
    numberArray.push(phoneNumber);

    for (var i = 0; i < numberArray.length; i++){
        if(numberArray[i] <= 100){
            document.getElementById('postAge').innerHTML = "Age: " + age;
        }
        if(numberArray[i] >= 100){
            document.getElementById('postPhoneNumber').innerHTML = "Phone Number: " + phoneNumber;
        }
    }

    var postFullName = document.getElementById("postFullName").innerHTML = firstName + " " + lastName;
    var postAddress = document.getElementById("postAddress").innerHTML = "Address: " + address;
  
}
