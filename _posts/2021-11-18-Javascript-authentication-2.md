---
layout: post
title: javascript authentication 2
---

Challenge này cần view source, đọc code từ hàm `login.js` để hiểu được flow của hàm này.
{% highlight ruby %}
function connexion(){
    var username = prompt("Username :", "");
    var password = prompt("Password :", "");
    var TheLists = ["GOD:HIDDEN"];
    for (i = 0; i < TheLists.length; i++)
    {
        if (TheLists[i].indexOf(username) == 0)
        {
            var TheSplit = TheLists[i].split(":");
            var TheUsername = TheSplit[0];
            var ThePassword = TheSplit[1];
            if (username == TheUsername && password == ThePassword)
            {
                alert("Vous pouvez utiliser ce mot de passe pour valider ce challenge (en majuscules) / You can use this password to validate this challenge (uppercase)");
            }
        }
        else
        {
            alert("Nope, you're a naughty hacker.")
        }
    }
}
{% endhighlight %}

code cấp mảng chứa username và pass.

Vòng For load theo từng kí tự của chuỗi TheLists. Dùng split tách chuỗi thành các khúc phân tách bằng dấu 2 chấm, phần trước là user, phần sau là pass



