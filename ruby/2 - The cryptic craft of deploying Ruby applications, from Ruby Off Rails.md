Hi there! This is email number 2 of 8 in the 'What you need to
know about Ruby' email course you signed up for on
RubyOffRails.com. If I am not creating value for you with these
emails, you can unsubscribe with 1 click at the end of this
email.

Once you get a program working locally, you need to get it on the
internet. So: deployment: a craft that's frustratingly difficult
to get into. After all, not too long ago, this was a
frustratingly colossal event. Back before Heroku, before Amazon
Web Services, and before Rackspace, we had to actually buy a
physical server and install stuff onto it. And somehow get an IP
address, so we needed space at a 'colo'.

Luckily for all of us, deploying is so easy, people now do it
often. I'll clone an entire application, and deploy a new feature
to it. Once approved, I'll shut it down. So freaking awesome.

Here's two quick wins on how to get your site from here (your
computer) to there (interwebs).

------
Heroku
------

Heroku is a developers dream; I use them for most projects
lately. Heroku Started as a Rails only solution, but can now host
any linux process. You can use them for Rails, Ruby, static HTML,
and the occasional Node/Clojure adventure.

Heroku is great for both small projects and very large projects
--- yours is likely small, so let's get started!

Your normal deployment to Heroku will look like this:

$ git push heroku master

This is telling git (your source control system) to push (send)
code to heroku (destination) from master (your local branch,
usually 'master' as you get started).

To make this happen, you should sign up for an account, and
download their 'toolbelt' ( https://toolbelt.heroku.com/ )

Then:

> cd project_directory

> heroku create $app_name

> git push heroku master

Literally you can open your site at $app_name.herokuapp.com

Like most things I love, it's free to get started, and most
Rubyists have used Heroku at one time or another.

I highly recommend this is your starting point; Create websites
here until you need something more, and then learn about
Capistrano.

----------
Capistrano
----------

If you are using a virtual private server to host your
application, you can get it to setup a folder structure using
Capistrano.

Note: when searching for capistrano, it helps to search 'ruby
capistrano' since Capistrano is a city in California. Similarly,
search for 'ruby unicorn' and 'ruby capybara'

Once your server is setup (see below), you'll run cap
deploy:setup and then: cap deploy

My normal server checklist:

* database server
* ruby
* logrotate
* web server (use nginx)
* application server (unicorn or puma)
* memcache
* redis
* setup a firewall

Each Ruby developer creates their own toolkit of Capistrano
'recipes' that do everything from installing Ruby scripts to
installing MariaDB and Redis.

Before going down the Capistrano road, I highly recommend
watching these two Railscasts recipes:

* 335-deploying-to-a-vps ( http://railscasts.com/episodes/335-deploying-to-a-vps )
* 337-capistrano-recipes ( http://railscasts.com/episodes/337-capistrano-recipes )

As for where to get your virtual servers? A quick guide:

* Rackspace: Pretty good, I've used and recommend. Pricing and
Performance are standard
* Amazon AWS: The Gold standard. Hint: Don't use us-east-1
* Digital Ocean: New player on the block, offers cheap and SSD
servers

I really love talking about Ruby. If you have any questions, or
just want to tell me what you found valuable from this email, hit
reply. I read every email and will get back to you.

- jesse
