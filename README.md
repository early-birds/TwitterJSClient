## Description
twitter-node-sdk aims to provide a complete, asynchronous client library for the Twitter API 1.1.

## Usage

  var Twitter = require('twitter-node-sdk');

  var config = {
    consumerKey: '{consumerKey}',
    consumerSecret: '{consumerSecret}',
    accessToken: '{accessToken}',
    accessTokenSecret: '{accessTokenSecret}',
    callBackUrl: '{callBackUrl}'
  };

  var twitter = new Twitter(config);

	twitter.getUserTimeline({ screen_name: 'BoyCook', count: '10'}, error, success);
	twitter.getMentionsTimeline({ count: '10'}, error, success);
	twitter.getHomeTimeline({ count: '10'}, error, success);
	twitter.getReTweetsOfMe({ count: '10'}, error, success);
	twitter.getTweet({ id: '1111111111'}, error, success);