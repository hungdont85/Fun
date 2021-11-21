---
layout: post
title: Javascript Webpack
---
Challenge build lại cve-2018-14732, thông qua lỗi tồn tại ở công cụ webpack. Còn webpack là gì thì google.

Để resolve chall này thì view source => cve khiến server trả về source thông qua webpack folder (dùng google chrom).
{% highlight ruby %}
export default {
  name: 'Duck',
  data () {
    return {
        // Did you know that comment are readable by the end user ?
        // Well, this because I build the application with the source maps enabled !!!

        // So please, disable source map when you build for production

        // Here is your flag : BecauseSourceMapsAreGreatForDebuggingButNotForProduction

        'msg': 'Quack quack !! :).'
    }
  }
}
{% endhighlight %}
