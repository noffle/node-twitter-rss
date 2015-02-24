# node-twitter-rss
Twitter RSS feed module for node

###Usage
```
var twitterRss = require('./twitter-rss')(CONSUMER_KEY,CONSUMER_SECRET,ACCESS_TOKEN,ACCESS_SECRET);

twitterRss.feed('Matthew_Reid', function(err, feed){
	if(err){
		console.log(err);
	}else{
		console.log(feed.render('rss-2.0'));
	}
})
```