<?php
header("Access-Control-Allow-Origin: *");
echo $SERVER["REQUESTS_METHOD"];

?>
request.onreadystatechange = function() {
    if (this.readyState == 4 && this.status == 200) {
      let response = JSON.parse(this.responseText);
      console.log(response);

     
    }
  };
