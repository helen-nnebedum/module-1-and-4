<!Doctype html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>form validation</title>
    </head>
    <body>
        <h1>
            Fill this Form
        </h1>
        <form name="myForm" onclick="validateform()" id="form"/>
            Name: <input type="text" name="uname" id="nameErr" required/>
            <br/>
            Phone Number: <input type="text" name="number" id="numberErr" required/>
            <br/>
            Email: <input type="text" name="email" id="emailErr" required/>
            <br/>
            <input  type="submit" value="submit" />
        </form>
        <script>
           var form = document.getElementById('form')

           form.addEventListener('submit',function(event){
             event.preventDefault() //prevent invalid submission

             var Name = document.getElementById('nameErr').value

             console.log(Name)

             var phoneNumber = document.getElementById('numberErr').value

             console.log(phoneNumber)

             var Email = document.getElementById('emailErr').value

             console.log(Email)

        })
        </script>
    </body>
</html>
