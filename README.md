# cwikibm
You can read this post here: https://hellotumo.com/typings/how-to-guides/bookmark-shortcut-to-clean-up-recipes-for-cooked-wiki/

*** 

I stumbled into [cooked.wiki](https://cooked.wiki), a lovely service that allows you to turn chaotic recipe web pages into clean and usable directions by adding “cooked.wiki/” in front of the URL.

Rather than typing that out repeatedly, I made a bookmarklet to handle the work. If you don’t know, a bookmarklet is a browser bookmark that uses JavaScript to manipulate a web page.

In this case, I grab the original recipe’s URL, add “https://cooked.wiki/” in front of it, and then launch a new window with that revised url.

To use the bookmarklet, you need to take a few steps:

1. Manually make a new bookmark in your browser.

2. Rather than type a URL into the URL field, you’re going to put in this JavaScript code:

javascript:(function(){let baseURL = window.location.href; let revisedURL = 'https://cooked.wiki/' + baseURL; window.open(revisedURL)})();
3. Then go to a recipe page and click on the bookmarklet you’ve created.

You can create a cooked.wiki account to save your favorites as you create them. I am at https://cooked.wiki/user/hellotumo. Here is an example of a “cooked.wiki” version of a mung bean egg recipe I tracked down: https://cooked.wiki/saved/8aa63401-d1c4-44be-a122-fa04e78246a9

