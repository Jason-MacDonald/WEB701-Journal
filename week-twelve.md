# Week Twelve

#### Project: Push Notifications

It's definately a call for concern when you initial research on a topic immediately describes itself as "actual rocket science". Push notifications are a little bit behind in the web world when compared to mobile apps, but it seemed appropriate for an auction website to let it's users know if they had won an auction item, that they had been outbid, and possibly also to notify the user if any events they responded to were starting soon.

Most articles I found on the topic mentioned to ensure users werent just blocking them notifications upon reaching the site by asking them to allow notifications at points where it made sence. For instance the first time a user bids on an auction or signs up for an event might then ask the user if they would like to be informed through notifications if they are outbid or there is any updated event information.

I also needed to deploy the website at a https location. This itself sunk a couple of days but was rather rewarding when finally deployed. I do need to look at a better workflow in the future as it is  bit fiddly working on the system. 

#### Implementing Push

Here I was thinking push notifications would be straight forward... I was wrong. The idea behind the system is reasonably straight forward.
* Register a service worker on the users browser,
* Ggenerate and save a subscription for the user,
* Send a message for the subscription(s) to a push notification server. 

... Oh how very wrong I was. The problem isn't the idea or flow of the system, but the elements required to ensure push notifications are secure and safe. We are essentially placing code within a browser that we can then call remotely so a robust system shouldn't really be a suprise. Several levels of encryption and key generation are required and there are many rules to follow. In reality, even that still isn't a problem.

The real problem I found was that I was just being left with no or limited error information. In fact I currently have push notifications working fine through firefox but not chrome. Unfortunately, all indications are suggesting that there is nothing wrong with the chrome version and I'm even getting a success message from the push server. 

So it took a huge amount of work and debugging and searching information just to get the actual notification to fire in firefox and I'm not sure how much more time I am going to be able to spend on notifications as we are nearing the end of the semester. I will likely finish off everything else I can and then come back to push notifications if time allows.



[Previous](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-eleven.md) |
[1](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-one.md) |
[2](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-two.md) |
[3](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-three.md) |
[4](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-four.md) |
[5](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-five.md) |
[6](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-six.md) |
[7](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-seven.md) |
[8](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-eight.md) |
[9](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-nine.md) |
[10](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-ten.md) |
[11](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-eleven.md) |
12 |
[13](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-thirteen.md) |
[14](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-fourteen.md) |
[15](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-fifteen.md) |
[16](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-sixteen.md) |
[Next](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/week-thirteen.md)

[Back to Contents](https://github.com/Jason-MacDonald/WEB701-Journal/blob/master/contents.md)
