---
layout: post
title: JS - Source - rootme
---
challen view source là thấy được password và cũng là `flag`
{% highlight ruby %}
function login(){
		pass=prompt("Entrez le mot de passe / Enter password");
		if ( pass == "123456azerty" ) {
		    alert("Mot de passe accepté, vous pouvez valider le challenge avec ce mot de passe.\nYou can validate the challenge using this password.");  }
		else {
		    alert("Mauvais mot de passe / wrong password !");
		}
	    }
{% endhighlight %}
