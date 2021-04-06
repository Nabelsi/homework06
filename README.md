# Homework 6: Javascript basics

##  Building our own search engine (with cheats)

Your browser comes with a predefined variable `location`, which contains the
URL of the site you're currently on. We can overwrite this variable to navigate
to other pages:

```javascript
location = "https://www.wikipedia.org";
```

In the file `search-engine.html` there is a text input and a button.

1. Create a Javascript function which takes the value of the input field and
   navigates to your preferred search engine with results for the input query.  
   Add a click handler to the button which calls this function.
1. Add a condition that if the user clicks on the button without having entered
   anything in the input field, the browser won't navigate anywhere.
1. Use the function
   [encodeURIComponent](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/encodeURIComponent)
   to sanitize the search query. That way you'll be able to include characters
   like `?`, `&` and `+` in it.
1. Add a `select` field where the user can choose between different search
   engines. Whichever search engine is currently selected, the user should be
   navigated to.
1. Make the site look a little bit prettier.

A few tips:

- You may change the HTML file
- Use `document.querySelector` to get the input and the select field in Javascript.
- Its values can be accessed with `field.value` (assuming you named the variable
  for the HTML element `field`).

Some example search engines with URLs:
```
DuckDuckGo    https://duckduckgo.com/?q=[your search term]
Google        https://www.google.com/search?q=[your search term]
Bing          https://bing.com/search?q=[your search term]
```
