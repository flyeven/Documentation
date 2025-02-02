---
title: Data Files
---

This feature is only available on Jekyll sites.
{: .info}

Data files are YAML, JSON or CSV files located in the `_data` directory.

Data files are another way over seperating your content from the HTML source code to help keep it organised.

In this example we'll have a CSV file of locations.

Create `_data/office_locations.csv` with the following contents:

{% highlight text %}
{% raw %}
latitude,longitude,name
-45.878760,170.502798,Dunedin Office
-41.286460,174.776236,Wellington Office
-46.098799,168.945819,Gore Office
-46.413187,168.353773,Invercargill Office
-35.117330, 173.267559, Kaitai Office
{% endraw %}
{% endhighlight %}

Now we can access this data in our site using `site.data.office_locations` like so:

{% highlight html %}
{% raw %}
...
  {% for location in site.data.office_locations %}
    <p>{{ location.name }}, {{ location.latitude }}, {{ location.longitude }}</p>
  {% endfor %}
...
{% endraw %}
{% endhighlight %}

Data files get their own tab in the Collections sidebar. Non-developers can edit these files using a visual interface:

![Data files](/img/jekyll/data_files.png){: .screenshot}
