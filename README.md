<html>

<head>
<script>



       /* 
    
 
    
 
     ======================================================================= 
    
 
    
 
     Title:  Alert message.
    
 
    
 
     Author: JavaScript Kit



     Modified by: Karie Funk
    
 
    
 
     Date: 5/31/2019 
    
 
    
 
     Class: WEB231 1.1 Values and Variables 
    
 
    Credit notice must stay intact for use
    //Visit http://javascriptkit.com for this script
 
     ======================================================================= 
    
 
    
 
     */ 



//specify message to alert
var alertmessage="This is an alert message \n https://github.com/kfunk17"


var once_per_session=1


function get_cookie(Name) {
  var search = Name + "="
  var returnvalue = "";
  if (document.cookie.length > ) {
    offset = document.cookie.indexOf(search)
    if (offset != -1) { // if cookie exists
      offset += search.length
      // set index of beginning of value
      end = document.cookie.indexOf(";", offset);
      // set index of end of cookie value
      if (end == -1)
         end = document.cookie.length;
      returnvalue=unescape(document.cookie.substring(offset, end))
      }
   }
  return retvalue;
}

function alertornot(){
if (get_cookie('alerted')==''){
loadalert()
document.cookie="alerted=yes"
}
}

function loadalert(){
alert(alertmessage)
}

if (once_per_session==0)
loadalert()
else
alertornot()

</script>

</head>




</html>
