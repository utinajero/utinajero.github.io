---
layout: post
title:  "How to install the unifi controller EASY!"
date:   2016-05-19 8:07:34 -0700
categories: jekyll update
---
How to setup Unifi controller on ubuntu 14.04.
[unifi-download-page]: https://www.ubnt.com/download/unifi/

{% highlight ruby %}
sudo apt-get update
sudo apt-get upgrade -y
sudo timedatectl set-timezone America/Los_Angeles
echo 'deb http://www.ubnt.com/downloads/unifi/debian stable ubiquiti' | sudo tee -a /etc/apt/sources.list.d/100-ubnt.list
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv C0A52C50
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv 7F0CEB10
sudo apt-get update
sudo apt-get install unifi -y
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll.
File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh].
If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
