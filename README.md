# Wikipedia Redirector For Getting The Old UI Back

## About

Wikipedia came out with a new layout and I think it is horrible. Wikipedia offer a method to disable this by creating an account and choosing your preferences. For those of us who don't want one damn more account to worry about I have created this repo to guide you through setting up your browser to negate the need to create an account.

## Credits

I did not come up with anything involved with this project simply packaged a tutorial credit where credit is due:

- REGEX pattern from Reddit user [OP_LOVES_YOU](https://www.reddit.com/user/OP_LOVES_YOU/)'s [post](https://www.reddit.com/r/wikipedia/comments/10fc9pn/comment/j50nkk9/?utm_source=share&utm_medium=web2x&context=3). <br>
- And the browser extension [Redirector-Firefox](https://addons.mozilla.org/en-US/firefox/addon/redirector/) / [Redirector-Chrome](https://chrome.google.com/webstore/detail/redirector/ocgpenflpmgnfapjedencafcfakcekcd) by [Einar Egilsson](https://einaregilsson.com/) (I have not tested Chrome version.)

## Setup

1. Install the extension:<br>[Redirector-Firefox](https://addons.mozilla.org/en-US/firefox/addon/redirector/)<br>[Redirector-Chrome](https://chrome.google.com/webstore/detail/redirector/ocgpenflpmgnfapjedencafcfakcekcd) (untested)

2. Download the redirect_to_old_wiki_layout.json file from this repo.

3. Left click the Redirector extension in your browser and choose **Edit Redirects**.<br>_You will see an example scrip here you may wish to disable it_

4. Click import and select the file you downloaded.

5. All going well you'll see a green success message! :)

6. Double check this rule is active then you're good to go.

## How it works

The extension will take any URL your enter into your browser and before senging the HTTP(s) request modify it to what every you ask it to based off a script.

Wikipedia offer a way to negate their UI update by adding the query to the end of a URL ``?useskin=vector``

The pattern here looks for any URL with ``http<whatever you want>wikipedia.org<whatever follows here>`` and adds that oh so important bit.

The script should hold up for anything you throw at it in your normal wiki surfing session XD.
