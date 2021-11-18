---
layout: post
title: JS - Authentication (rootme)
---
Challenge này tương tự challenge trước ~ cũng F12 để mò

Sẽ có file `login.js` để vào xem code
{% highlight ruby %}
function Login(){
	var pseudo=document.login.pseudo.value;
	var username=pseudo.toLowerCase();
	var password=document.login.password.value;
	password=password.toLowerCase();
	if (pseudo=="4dm1n" && password=="sh.org") {
	    alert("Password accepté, vous pouvez valider le challenge avec ce mot de passe.\nYou an validate the challenge using this password.");
	} else { 
	    alert("Mauvais mot de passe / wrong password"); 
	}
}
{% endihighlight %}
giá trị login được lấy từ 2 biên  `pseudo` và `password`.
