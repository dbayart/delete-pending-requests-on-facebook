# How to delete all your pending friend's requests on Facebook ?
This is a short tutorial to show you how to execute a small script to delete all your pending friend's requests at once.

This script works well with the _Google Chrome_ webbrowser.

##### Bug with Firefox
There is a bug with Firefox.
Only half requests are deleted with that script.

#### English langage required !
This script works only if your Facebook is displayed in english !  
To change the langage, set the display langage setting to `english` here : https://www.facebook.com/settings?tab=language

### Steps
1. **Go to the Friend's requests page**  
You'll find that page here : https://www.facebook.com/friends/requests/?fcref=jwl  
Then scroll down a bit and click on the `Show more requests` link until there is no more requests to display (it depends on how much pending requests you have).


2. Open the Javascript Console  
Sometimes it may ask you to type some words to allow you to execute a script command.  
This is to prevent you to execute bad scripts found somewhere, 
  1. **Chrome users**  
Press : `Ctrl` + `Shift` + `J` (Windows) / `Cmd` + `Opt` + `J` (Mac)

  2. **Firefox users**  
Press : `Ctrl` + `F4`

3. Execute the script
  ```javascript
  inputs=document.getElementsByTagName('button'); for(i in inputs){if(inputs[i].innerHTML == 'Delete Request' && inputs[i].id != "") {inputs[i].click();}}
  ```
  1. Copy this script
  2. Paste it to your Javascript Console
  3. Execute it by pressing Enter




#### Result
You should see all the "Delete Request" button turning into a "Mark as Spam" button.  
Done. :+1:
