<?php

$myfile = fopen("location.txt", "w");
$txt = "lat: " . $_GET["lat"] . "\nlong: " . $_GET["long"]."\n IP:" . $_SERVER["REMOTE_ADDR"];
fwrite($myfile, $txt);
fclose($myfile);


?>