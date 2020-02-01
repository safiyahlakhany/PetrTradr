# PetrTradr
_Are you looking trade your graduation Petr for a Thanos Petr? Do you have a drop to get to tomorrow but you tend to forget? Want an app to keep track of your Petrs? If so, PetrTradr has got you covered._

Awarded 1st Place Overall Hack at HackUCI 2020

---
## Inspiration
A little over a year ago, stickers depicting UCI's mascot, Peter the Anteater, were released. The "petr stickers" forever changed culture at UCI. Hundreds of students would drop everything and run at the news of a "petr drop". We noticed that on websites, like Facebook and Reddit, students would often make posts asking for others if they want to trade the stickers that they have currently collected. The wave also inspired many UCI students to keep a portfolio of their stickers, and this led to a community-wide collective goal that inspired students to collect all of the "petrs". We turned this idea into an iOS app on your phone.

## What it does
PetrTradr allows users to keep track of their "petr" stickers collection on their in-app profile. On a user's profile, they can see which and how many stickers they own to finish their Petr portfolio.  Additionally, PetrTradr allows users to make trading requests where they can indicate which stickers they intend to trade and which they desire. Users can send a text message through the app to another user if they are looking to trade with them. Furthermore, users can create a push notification that will remind them when the next "petr" drop will occur. So much "petr", so little time.

<img src='http://g.recordit.co/jWVSeMQqfJ.gif' title='Video Walkthrough' width='' alt='Video Walkthrough' />

## How we built it
PetrTradr is an iOS app built using Swift. We used the Parse framework to connect our app to our database (MongoDB) and for user account creation. Additionally, we used the Twilio API for a messaging featured. We also utilized Alamofire for network requests.

## Challenges we ran into
Because Xcode projects are not GitHub friendly, we encountered numerous merge conflicts. In addition, we initially intended for the user to be reminded with text notifications via the Twilio API. However, in order to schedule a reminder for the future, we needed to have a concurrent Python server running that would send the text notification at a later date. However, we could not get Xcode to connect to our server and post an API request in time, so opted out for UNUserNotificationCenter to send the user local notifications for the future instead. As of now, the user will still receive text messages via the Twilio API, but only when they want to send another user a request message to trade "petrs".

## Accomplishments that we're proud of
PetrTradr is technically complex; it relies on an external database to store a user's account name, encrypted password, "petr" drop reminders, outgoing trade requests, and stickers collected. It utilizes a third party API - Twilio - in order to allow the user to send other users text messages for a "petr" trade exchange. It also sends push notifications to the user's device when they want to be reminded of an upcoming "petr" drop in the future. On top of the multiple back-end interfaces, we implemented a very user-friendly and physically appealing UI. Each user is given a profile of which "petr" stickers they have, that are able to light up/ gray out based on ownership. Beautiful inside and out!

## What we learned
We were all able to experiment with new tools and technologies that we hadn't previously been exposed to. A few of us were new to Parse, and all of us were unfamiliar with Twilio API. We most certainly all got a lot better working with iOS, and merging on GitHub. In general, we all came out with a sense of pride and excitement to apply these new skills to our programming lives!

## What's next for PetrTradr
We would love to implement more features on PetrTradr such as the ability to host petr drops and notify users internally within the app. We would love to have an admin side of the app, primarily for the Petr's to drop within there, instead of instagram. Taking it one step further, an implementation of a social forum would be amazing. 
We hope to release PetrTradr on the App Store as well as the Play Store for UCI students to use for years to come. 

 Devpost: https://devpost.com/software/tradr-u10jg4
 
 Demo: https://www.youtube.com/watch?v=8qXXXDt4des
