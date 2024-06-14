---
layout: post
title: JS - Authentication (rootme)
---
Challenge này tương tự challenge trước , cũng F12 để mò

hoặc bắt request lúc bấm nút login thì server trả về dạng link: http://challenge01.root-me.org/web-client/ch9/login.js

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
{% endhighlight %}
giá trị login được lấy từ 2 biến  `pseudo` và `password`.
