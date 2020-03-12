# get-random-tweet-api
> The Get Random Tweet API lets you get one random tweet of any public profile on Twitter.

- Really simple and easy
- Random sample of any tweet in whole user timeline
- No login or Twitter API key required
- No duplicate samples

---

## Live demo

https://marcosogsantos.github.io/randombird/

## Description

Normally to get random samples of a twitter account you need to resquest "chunks" of user timeline until store all tweets and then get a random sample of this stored data. That method could be great for relative short user timelines and for dedicate in specifics profiles, but not for really big ones and generalized group of users.

With a simple "trick", this API let's you get one random tweet of a public profile with any size timeline, avoiding duplicates and without you store any data.

---
## Example
Request
```html
https://get-random-tweet-api.herokuapp.com/?user=realdonaldtrump
```
Result
```javascript
{
  "text":
      "Going to Louisiana on Friday night for a big Republican Rally. Keep Democrat Governor Edwards under 50%, force a runoff, and have a great new Republican Governor! Voting on Saturday. Information for Rally to follow.",
  "link":
      "https://twitter.com/realDonaldTrump/status/1180899945701879808",
   "date":
      "06/10/2019",
   "retweets":
      16084,
    "favorites":
      61389,
    "geo":
      "",
    "user":
      "realdonaldtrump"
}
```
---

## Observations
Because this method don't require a Twitter API Key, I don't have a request limit number (probably this will come from host ip ban by some sort of Twitter DDOS Security - that must be a big number - and the host free traffic limits). 

For now, the backend dont use a ideal database system because it work with small and simple data (I thought that would be overwork) buts seems work fine.

So feel free to push this limits. Report me any issue or idea.
