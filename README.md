# updooter
A JS url to automatically upvote all comments and posts in a `reddit` page.

Just copy/paste the following url in your browser window, or bookmark it and it will upvote all comments and posts in the current page.

```
javascript:(function()%7Bvar q%3D%5B%5D%3B%24(%27.up%27).each(function()%7Bvar that%3Dthis%3Bvar f%3Dfunction(index)%7B%24(that).trigger(%27click%27)%3B%24(that).trigger(%27mousedown%27)%3BsetTimeout(function()%7Bif(q%5Bindex%5D)%7Bq%5Bindex%5D(index%2B1)%3B%7Delse%7Bif(upVoteTimer)%7Bwindow.clearTimeout(upVoteTimer)%3B%7D%7D%7D,500)%3B%7D%3Bq.push(f)%3B%7D)%3Bvar upVoteTimer%3Dwindow.setTimeout(function()%7Bq%5B0%5D(1)%3B%7D,50)%3B%7D())%3B
```

Some browsers may remove the `javascript` prefix so doublecheck!

<b>NOTE:</b> ONLY works on old `reddit` layout
