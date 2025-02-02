---
title: Custom Routes
---

Custom Routes are only available on the CloudCannon Basic plan and above and sites hosted by CloudCannon.
{: .info}
{: .warning}

Custom routes allow you to specify the routes you want authenticated, and keep the rest public.
This feature is ideal for staff or special subscriber sections of your site.

By default, all routes are authenticated.
{: .info}

To specify custom authenticated routes for your site:

1. Create a file named `auth-routes.txt` in the root folder
2. Add the routes you want to this file, one on each line.

CloudCannon supports wildcards, allowing you to specify child folders or multiple files.

In the following example, visitors will have to log in to access `/internal-news.html` and anything inside `/staff`. Everything else is public.

{% highlight text %}
/internal-news.html
/staff/*
{% endhighlight %}
