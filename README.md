# Cookie
&lt;?php $cookie_name = "user"; $cookie_value = "John Doe"; setcookie($cookie_name, $cookie_value, time() + (86400 * 30), "/"); // 86400 = 1 day ?> &lt;html> &lt;body>  &lt;?php if(!isset($_COOKIE[$cookie_name])) {   echo "Cookie named '" . $cookie_name . "' is not set!"; } else {   echo "Cookie '" . $cookie_name . "' is set!&lt;br>";   echo "Value is: " . $_COOKIE[$cookie_name]; } ?>  &lt;/body>
