# getCookie
this is a script from w3schools.com, all credits belong to w3schools.com

link of the script: https://www.w3schools.com/js/js_cookies.asp

// just feed the cookie name as parameter, and it will output the cookie value

```
function getCookie(cname) {
    var name = cname + "=";
    var decodedCookie = decodeURIComponent(document.cookie);
    var ca = decodedCookie.split(';');
    for(var i = 0; i <ca.length; i++) {
        var c = ca[i];
        while (c.charAt(0) == ' ') {
        c = c.substring(1);
        }
        if (c.indexOf(name) == 0) {
        return c.substring(name.length, c.length);
        }
    }
    return "";
}
```
