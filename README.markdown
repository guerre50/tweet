# Tweet!
#### Put twitter on your website with tweet!, an unobtrusive javascript plugin for jquery.

## Important note about Twitter's API changes in 2013

Twitter has <a href="https://dev.twitter.com/docs/api/1.1/overview">discontinued
its unauthenticated v1.0 API</a>.

<em>Victor:</em> Due to that and thanks to Jason Mayes <a href="http://jasonmayes.com/projects/twitterApi/#sthash.Nvi8TTYJ.dpbs">TwitterFetcher</a> I have modified the original project to work again. Just create your widget and add its id as a parameter (widget_id) when initializing the plugin 


## Create a widget:

* go to <a href="https://twitter.com/settings/widgets/new">https://twitter.com/settings/widgets/new</a>
* configure your widget and click "Create widget" button
* in the embeddable code generated look for <b>data-widget-id</b> and pass its value as a new parameter <b>widget_id</b>:

## Demos & examples

See [https://dl.dropboxusercontent.com/u/5476179/tweet/index.html](https://dl.dropboxusercontent.com/u/5476179/tweet/index.html), or the bundled `index.html` file.

## Source

[Download tarball](http://github.com/seaofclouds/tweet/tarball/master)

## Features

  * small size and fast download time
  * will not slow down or pause your page while tweets are loading
  * display up to 100 tweets, as permitted by the twitter search api
  * display tweets from a twitter search, or from your own feed
  * optional verb tense matching, for human readable tweets
  * optionally display your avatar
  * optionally display tweets from multiple accounts!
  * automatic linking of @replies to users’ twitter page
  * automatic linking of URLs
  * automatic linking of #hashtags, to a twitter search of all your tags
  * converts <3 to a css styleable ♥ (we ♥ hearts)
  * customize the style with your own stylesheet or with other jquery plugins
  * customize the layout with a user-defined template function
  * supports RequireJS and other AMD-compatible javascript loaders
  * available on [cdnjs](http://cdnjs.com)

## Usage

1. Get [JQuery](http://jquery.com/). In these examples, we use [Google's AJAX Libraries API](http://code.google.com/apis/ajaxlibs/).


2. include jQuery and jquery.tweet.js files in your template's `<head>`.

        <script language="javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.6.4/jquery.min.js" type="text/javascript"></script>
        <script language="javascript" src="/tweet/jquery.tweet.js" type="text/javascript"></script>

3. Also in `<head>`, Initialize tweet! on page load with your Username and other options

        <script type='text/javascript'>
            jQuery(function($){
                $(".tweet").tweet({
                    join_text: "auto",
                    avatar_size: 32,
                    count: 3,
                    widget_id: "319141590008467456",
                    loading_text: "loading tweets..."
                });
            });
        </script>

4. In `<body>`, include a placeholder for your tweets. They'll get loaded in via JSON. How fancy!

        <div class="tweet"></div>

5. Style with our stylesheet in `<head>`, or modify as you like!

        <link href="jquery.tweet.css" media="all" rel="stylesheet" type="text/css"/>


### Contribute

Bring your code slinging skills to Github and help us develop new features for tweet!

[Github project page](http://github.com/seaofclouds/tweet/)

    git clone git://github.com/seaofclouds/tweet.git

Report bugs at http://github.com/seaofclouds/tweet/issues

### Licensed under the MIT

[License text](http://www.opensource.org/licenses/mit-license.php)

<hr>

[![](http://api.coderwall.com/purcell/endorsecount.png)](http://coderwall.com/purcell)
