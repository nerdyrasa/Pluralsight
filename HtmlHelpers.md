## Build an MVC Helper

Replace 

```
<img src="../Images/someImage.jpg"
	 alt="Some descriptive text here"
	 class="img-responsive img-rounded"
	 id="imgSomeImage"
	 data-action="moreInfo" />
```
with this:
```
@Html.Image("../Images/someImage.jpg",
			"Some descriptive text here",
			"img-responsive img-rounded",
			"imgSomeImage",
			new { data_action = "moreInfo" })
```

### Use StringBuilder class

How-to
1. Build a static class
2. Add static method to return an MvcHtmlString
3. Use StringBuilder class to build HTML
4. Return the HTML as an MvcHtmlString

Advantages:
1. Familiar class
2. Good for string concatenation

Disadvantages:
1. Lots of chance to introduce errors: forget to close tags, mismatch quotes, etc

### Use TagBuilder class

1. TagBuilder is designed specifically to create HTML tags
2. Many


### Which one is best to use?

### The MvcHtmlString class

### Add HTML attributes dictionary (anonymous object)


