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

code cấp `array` chứa username và pass.

Vòng `For` chạy để lấy các phần tử trong array ra => đem so sánh với username người dùng nhập vào => Nếu không tồn tại trong `array` thì thực hiện thứ trong hàm `if` => tách array bằng hàm `split`.



