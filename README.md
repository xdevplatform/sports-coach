# Hide Replies Sports coach

Keep your conversation on topic in one single step!

## What is it?

Twitter users sometimes want to keep their conversations focused on the main topic they are discussing. The Hide Replies feature in Twitter API v2 enables you to build an app to help Twitter users have better control over the topics discussed in a conversation.

## How does it work?

The flow of this app is straightfoward:

1. The app asks the user to provide a Twitter link to one of their recent conversations.
1. The app uses [Recent search](https://developer.twitter.com/en/docs/twitter-api/tweets/search/api-reference/get-tweets-search-recent) to retrieve the entire conversation, including its replies. The app requests the [Tweet annotations](https://developer.twitter.com/en/docs/twitter-api/annotations/overview) for each reply.
1. Each reply's annotation is compared against any of the Sports Tweet annotations domains.
1. If a reply doesn't match any of the known Sports domains, the app shows a prompt to hide it using [Hide replies](https://developer.twitter.com/en/docs/twitter-api/tweets/hide-replies/introduction) 

## Can I clone this project?

Yes! [Remix this project](https://glitch.com/remix/#!/twitter-hide-replies-annotations-v2) to see the code and change it to your liking.

In order to make the app work for you, you will need to [get access to the Twitter API](https://t.co/signup). It's fast, immediate, and free.
