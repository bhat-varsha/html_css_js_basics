A form in HTML is used to collect user input.

input control=These are the fields inside the form where users enter data.
input type ="text" "password" "email" "number" "date" "checkbox" "file"

🔘 Radio (choose one)
<input type="radio" name="gender">
_______________________________________________________
button = Sends form data
three valid button types
1.submit=This submits the form and  Sends data to backend
2.reset=This clears all inputs in the form
3.button (nothing does by defalu )#it is used in java script

<button type="submit">Submit</button. for those 3 
if we dont have analyse button types , we have to create using name+value
<button type="submit" name="action" value="analyse">Analyse</button>
_______________________________________________________

Label = Just text describing the input
_______________________________________________________
Form Attributes
1.action =  Where data is sent (server URL)
<form action="/search">

2.method
GET:
Data visible in URL
Used for search

POST:
Data hidden
Used for login, sensitive data

3.name:This is the key sent to backend
<input name="userid">
