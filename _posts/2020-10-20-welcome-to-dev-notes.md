---
layout: post
title: Welcome to DevNotes
date: 220-10-20 06:44:00 +0530
categories: jekyll general
---

__DevNotes__ is a [Jekyll](https://jekyllrb.com) based template for quickly creating a note making platform for developers.

A developer's note is different than the general note which contains mostly text. The note of a developer contains code snippet, multimedia like images and video, hyperlinks etc.

This template will help you create your own note making platform.

## Note with code snippet

The most general form of note is the one which contain any code snippet.

For example, if you are writing a note which has some text and code snippet and you want to share with your friends.

Then, you can write such note through this platform as:

{% highlight text %}
I was working on some code and found following code snippet interesting.

```c
#include <stdio.h>

int main() {
  printf("Namaste, DevNotes!");
}
```

This program has no return statement and it is still working.
Magic!
{% endhighlight %}

This platform will render the code snippet of above note as below with grey background:

```c
#include <stdio.h>

int main() {
  printf("Namaste, DevNotes!");
}
```

The another format for code snippet is using `highlight` block as below:

{% highlight text %}
{% raw %}
{% highlight c %}
#include <stdio.h>

int main() {
  printf("Namaste, DevNotes!");
}
{% endhighlight %}
{% endraw %}
{% endhighlight %}

The benefit of using `highlight` syntax is that we can specify line numbers as well like below:

{% highlight text %}
{% raw %}
{% highlight c linenos %}
#include <stdio.h>

int main() {
  printf("Namaste, DevNotes!");
}
{% endhighlight %}
{% endraw %}
{% endhighlight %}

The result is :

{% highlight c linenos %}
#include <stdio.h>

int main() {
  printf("Namaste, DevNotes!");
}
{% endhighlight %}

## Customizations

To customize your notes, you need to have basic understanding of [Jekyll](https://jekyllrb.com) which is very easy framework to learn and would be easy if you already know about HTML, CSS and JavaScript.

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll.

## Bugs or Feature request

If you found any bug or have feature request, consider checking the [GitHub repo](https://github.com/brgprojects/devnotes) and file an issue.

Happy note making!
