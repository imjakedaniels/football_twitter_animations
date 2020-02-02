<h1 style="font-weight:normal" align="center">
  &nbsp;Visualizing Twitter Chatter during Football&nbsp;
</h1>

## Scraping & animating a basketball game using `{rtweet}` & `{gganimate}` 

<p align="center">
  <img src="https://github.com/imjakedaniels/football_twitter_animations/blob/master/animations/packers_anim.gif">
</p>

**Data**: 
```{r}
tweet_keywords <- "#GBvsDET OR #ThePackIsBack OR #PutCheeseOnEverything OR #GoPackGo OR @packers OR #greenbaypackers OR #packers OR packers"

rtweet::search_tweets(tweet_keywords,
                      n = 18000*5, 
                      include_rts = FALSE,
                      retryonratelimit = TRUE,
                      type = "recent")
```

**Notebook**: the graph is created using RMarkdown. See the code [here](https://github.com/imjakedaniels/raptors_animation/blob/master/football_animation_notebok.Rmd).

## Details

I've been trying to apply some learning from my Leafs' Twitter visualizations into other sports. Football seems like it has distinct events that would be great to indicate. 

On first efforts, I'm not sure the words were very specific/good. Visual does look good. May return to this in the 2020-2021 season.

## Requirements

```
library(tidyverse) # for the basics
library(rtweet) # for tweets
library(lubridate) # for date manipulation
library(tidytext) # for tokenizing
library(gganimate) # for gifs
library(rvest) # for scraping html
library(png) # for image manipulation
library(grid) # for custom plot manipulation
library(extrafont) # for nice fonts
library(ggtext) # for adding colour in plot titles
```

## See more 

See more animations in the /animations folder.

[Twitter][Twitter] :speech_balloon:&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[LinkedIn][LinkedIn] :necktie:&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[GitHub :octocat:][GitHub]&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Reddit][Reddit] :link:

</div>

<!--
Quick Link 
-->

[Twitter]:https://twitter.com/datajake
[LinkedIn]:https://www.linkedin.com/in/imjakedaniels/
[GitHub]:https://github.com/imjakedaniels
[Reddit]:https://www.reddit.com/user/imjakedaniels
