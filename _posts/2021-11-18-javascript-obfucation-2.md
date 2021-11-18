---
layout: post
title: javascript obfucation 2
---
View source để xem code như nào
{% highlight ruby %}
<script type="text/javascript">
	var pass = unescape("unescape%28%22String.fromCharCode%2528104%252C68%252C117%252C102%252C106%252C100%252C107%252C105%252C49%252C53%252C54%2529%22%29");
</script>
{% endhighlight %}
hiểu đc script trên thì ăn đc bài này.

Như bài trước => dùng `unescape` 3 lần => khúc cuối dùng `fromCharCode` để chuyển từ Unicode sang kí tự.
