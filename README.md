# get-random-tweet-api
> This API lets you get one random tweet of any public profile on Twitter.

- Really simple and easy
- Random sample of any tweet in whole user timeline
- No login or Twitter API key required
- ~~No duplicate samples~~

---

## Live demo

https://marcosogsantos.github.io/randombird/

## Description

Normally to get random samples of a twitter account you need to resquest "chunks" of user timeline until store all tweets and then get a random sample of this stored data. That method could be great for relative short user timelines and for dedicate in specifics profiles, but not for really big ones and generalized group of users.

With a simple "trick", this API let's you get one random tweet of a public profile with any size timeline and ~~avoiding duplicates~~.

---
## Example
Request
```html
https://get-random-tweet-api.herokuapp.com/?user=BarackObama
```
Result
```javascript
{
  "contributors": null,
  "coordinates": null,
  "created_at": "Fri Jun 08 16:01:17 +0000 2018",
  "entities": {
    "hashtags": [],
    "symbols": [],
    "urls": [
      {
        "display_url": "twitter.com/i/web/status/1…",
        "expanded_url": "https://twitter.com/i/web/status/1005117568913412098",
        "indices": [
          117,
          140
        ],
        "url": "https://t.co/l79o6OyNAT"
      }
    ],
    "user_mentions": []
  },
  "error": false,
  "favorite_count": 1042438,
  "favorited": false,
  "geo": null,
  "id": 1005117568913412098,
  "id_str": "1005117568913412098",
  "in_reply_to_screen_name": null,
  "in_reply_to_status_id": null,
  "in_reply_to_status_id_str": null,
  "in_reply_to_user_id": null,
  "in_reply_to_user_id_str": null,
  "is_quote_status": false,
  "lang": "en",
  "place": null,
  "possibly_sensitive": false,
  "retweet_count": 217044,
  "retweeted": false,
  "source": "<a href=\"http://twitter.com/download/iphone\" rel=\"nofollow\">Twitter for iPhone</a>",
  "text": "“Low plastic stool, cheap but delicious noodles, cold Hanoi beer.” This is how I’ll remember Tony. He taught us abo… https://t.co/l79o6OyNAT",
  "truncated": true,
  "user": {
    "id": 813286,
    "id_str": "813286"
  }
}
```
---
