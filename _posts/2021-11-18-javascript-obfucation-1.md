---
layout: post
title: javascript obfucation 1
---
View source challenge thì có script để verify.
code
{% highlight ruby%}
pass = '%63%70%61%73%62%69%65%6e%64%75%72%70%61%73%73%77%6f%72%64';
h = window.prompt('Entrez le mot de passe / Enter password');
if(h == unescape(pass)) {
    alert('Password accepté, vous pouvez valider le challenge avec ce mot de passe.\nYou an validate the challenge using this pass.');
} else {
    alert('Mauvais mot de passe / wrong password');
}
{% endhighlight%}
dùng hàm `unescape` của js trên devtool để lấy flag.
