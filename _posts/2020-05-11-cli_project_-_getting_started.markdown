---
layout: post
title:      "CLI Project - Getting Started"
date:       2020-05-11 04:21:18 +0000
permalink:  cli_project_-_getting_started
---


I hope that in reading this, you will feel more confident about beginning your CLI project. My target audience are students learning how to scrape and how to build a CLI app. If that does not apply to you, I hope that you can take away some tips on organization!

For me, the hardest part of this project was figuring out how to get started. The first factor that played into my discomfort, and most likely several of you at this stage, was that I had never attempted - or even dreamt of attempting - to create anything from absolute scratch via coding. Needless to say, I experienced my fair share of anxiety. Here’s what I’ve learned: the tools and resources that have gotten you to the point of the CLI project are sufficient enough to get you through the project. Getting to this point, I’m sure, has not been entirely easy. Else, you wouldn’t be reading this, right? However, there is hope.

I would highly recommend the following resources:

1. The Learn Instruct [app](https://instruction.learn.co/student/video_lectures#/) is a fantastic tool. There, there are many videos - similar to the recorded lectures that are provided in your cohort! This helped me tremendously by providing several approaches to completing the project. Unfortunately, I don't believe students outside of Flatiron School can access it...yet.

2. Watch the video of your cohort lead’s lecture on scraping and any related lectures, such as gems.

3. Google is your friend. If you have not already, practice making better searches. One of mine for this project was:
“CLI project blog scraping Learn” : this is how I discovered the Learn Instruct app.

Here are some tips to stay organized during the project:

1. Start by brainstorming. It is very easy to get carried away with the bells and whistles. Take some time to jot down what the bare requirements are, figure out how to complete those first, then add embellishments if you have the time to do so.

2. Take notes: I kept a project journal that housed my ideas, processes, questions, and resources. This helps you to keep track of your thought process, which is especially helpful if you get lost in the dense fog of debugging code.

Bonus: this really helped me to understand where to look for the problem when debugging:

Sample error:

```
Welcome to the Zeitz Museum of Contemporary Art Africa Features (MOCAA) App!
What is your name?
amal
Hi, amal.
The scraping process will commence shortly. Your patience is appreciated.
Traceback (most recent call last):
        2: from ./bin/zm_features_run:7:in `<main>'
        1: from /home/beloved-edition-9426/temporary/zm_features/lib/zm_features/cli_class.rb:105:in `run'
/home/beloved-edition-9426/temporary/zm_features/lib/zm_features/cli_class.rb:33:in `begin_to_scrape': uninitialized
 constant ZMFeatures::CLI::ZMFeaturesScraper (NameError)
```

To find the problem, work backwards! Look first at the ZMFeaturesScraper, then go up to the next line at the begin_to_scrape method. It is uninitialized. How would I gain access to a method that’s not in my present class? One way to do it would be to require the file that houses the method named there. If you name your elements well, it will help you later on if you run into a problem. Since I see “scrape”, I’ll go to my environment file and make sure the scrape file is required using:

#require_relative “./folder_name/file_name”

For example:
#require_relative "./zm_features/scraper_class"

I hope you find this helpful. Thanks for stopping by!

