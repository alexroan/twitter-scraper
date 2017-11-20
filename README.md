# twitter-scraper
Grab tweets from a user's public profile without api credentials

## Installation

### Composer

composer require alexroan/twitter-scraper

## Usage

```php
//get feed
$feed = Twitter_Scraper::get_feed('alex_roan');

//loop through posts
foreach($feed as $tweet){ 

    //tweet id
    $id = $tweet->id;

    //username of tweeter
    $username = $tweet->username;

    //bool whether retweet or not
    $is_retweet = $tweet->is_retweet;

    //body text of tweet
    $text = $tweet->text;

    //time tweeted
    $time = $tweet->time;

    //any media in tweet
    $media = $tweet->media;

    //number of replies
    $reply = $tweet->reply;

    //number of retweets
    $retweet = $tweet->retweet;

    //number of favourites
    $favourite = $tweet->favourite;

}
```
