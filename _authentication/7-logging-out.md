---
title: Logging out
---

Once a user is authenticated, they can log out at `<your-domain>/logout`. You can provide a log out button on your authenticated pages with this link.

{% highlight html %}
<a href="/logout">Log out</a>
{% endhighlight %}

---

## Custom Routes

CloudCannon sets a cookie when the user is authenticated.
Use this to show the log out button for authenticated users on public pages, and hide it otherwise.

No sensitive authentication data is exposed through cookies.
{: .info}

The cookie is used to set a class on the body. The CSS will show the log out button with this class.

{% highlight javascript %}
var isAuthenticated = document.cookie.indexOf("authenticated=true") >= 0;

if (isAuthenticated) {
  document.body.className += " authenticated";
}
{% endhighlight %}

{% highlight css %}
.logout {
  display: none;
}

.authenticated .logout {
  display: block;
}
{% endhighlight %}

{% highlight html %}
<a href="/logout" class="logout">Log out</a>
{% endhighlight %}
