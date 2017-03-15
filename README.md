# Blogger Conditional Tag — b:if and b:else

Blogger Conditional Tag এর সাথে পরিচিত হোন

Blogger এর আছে বিশেষ `<b:if>` এবং `<b:else/>` tags.

`<b:if>` ও `<b:else/>` কাজ করবে শুধুমাত্র XHTML এ করা কোনো Blogger blog এ।

এমনকি Layout এর মাধ্যমে HTML/JS widget দিয়েও এটি করা যাবে না।

## List of `<b:if>` conditions

* Item
* Static
* Index
* Archive
* Homepage
* Specific URL
* Error Page
* Backlink
* Display Name
* Number of Comments
* Jump Link
* Commenting Enabled
* Others


### ITEM

Show content only on item page (every single post):

```
<b:if cond='data:blog.pageType == "item"'>...content...</b:if>
```

### STATIC
Show content only on static page(s):
```
<b:if cond='data:blog.pageType == "static_page"'>...content...</b:if>
```

### INDEX

Show content only on index page (sorted by label and date):

```
<b:if cond='data:blog.pageType == "index"'>...content...</b:if>
```

```
For instance, try this URL pattern:
[your_blog_url]/search/label/[YOUR_LABEL]
It will show your post(s) list with a particular [YOUR_LABEL] label.

change the [your_blog_url] with your own blog URL, such as: mysupersweetblog.blogspot.com or your custom domain blog URL.
change the [YOUR_LABEL] with your own label.
```

### ARCHIVE

Show content only on archive page (your blogroll — sorted by date):

```
<b:if cond='data:blog.pageType == "archive"'>...content...</b:if>
```

```
For instance, try this URL pattern:
[your_blog_url]/2014/11
It will show your post(s) list you wrote in November ( 11 ) of 2014.
Also, change the [your_blog_url] with your actual blog URL. 
```

### HOMEPAGE

Show content only on homepage URL of the blog:

```
<b:if cond='data:blog.url == data:blog.homepageUrl'>...content...</b:if>
```

### SPECIFIC URL

Show content only on a specific URL on the blog:

```
<b:if cond='data:blog.url == "specific-URL-on-the-blog"'>...content...</b:if>
```

We need to put complete URL and protocol for that, such as:

```
http://mysupersweetblog.blogspot.com/2002/01/hello_hoho.html
```

Do not use relative URL, like just /2002/01/hello_hoho.html. 

### ERROR PAGE

Show content on the error page of the blog (404 - not found page):

```
<b:if cond='data:blog.pageType == "error_page"'>...404 note content...</b:if>
```

There's the predefined elements and styling provided by Blogger for that.

They're the elements starting with class name `status-msg-`.

You can search them on your XHTML.

But, if you wanna modify the custom error page, use that conditional statement to make the additional element(s)/CSS/JS appear/run only for that criteria. 

### BACKLINK

Show content only on post(s) which is/are showing backlink:

```
<b:if cond='data:post.showBacklinks'>...content...</b:if>
```

### DISPLAY NAME

Show content only on post(s) which is/are showing specific display name (such as the post's author):

```
<b:if cond='data:displayname == "specific-name"'>...content...</b:if>
```


### NUMBER OF COMMENTS

Show content only on post(s) which has/have specific number of comment(s):

```
<b:if cond='data:post.numComments == [number_here]'>...content...</b:if>
```

### JUMP LINK

Show content only on post(s) which has/have jump link (the "read more" link):

```
<b:if cond='data:post.hasJumpLink'>...content...</b:if>
```

### COMMENTING ENABLED

Show content only on post(s) which is/are comment enabled:

```
<b:if cond='data:post.allowComments'>...content...</b:if>
```

### OTHERS

There are plenty other of conditions. But they're "deeper", sort of speak.

These are some of them:

```
<b:if cond='data:blog.metaDescription'>
<b:if cond='data:mobile'>
<b:if cond='data:title'> or <b:if cond='data:title != ""'>
<b:if cond='data:showThumbnails == "false/true"'>
<b:if cond='data:showSnippets == "false/true"'>
<b:if cond='data:post.thumbnail'>
<b:if cond='data:display == "list"'>
<b:if cond='data:blog.url == data:label.url'>
<b:if cond='data:showFreqNumbers'>
<b:if cond='data:useImage'>
```

Plus others...













* [Dropwizard](http://www.dropwizard.io/1.0.2/docs/) - The web framework used
* [Maven](https://maven.apache.org/) - Dependency Management
* [ROME](https://rometools.github.io/rome/) - Used to generate RSS Feeds

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to anyone who's code was used
* Inspiration
* etc

