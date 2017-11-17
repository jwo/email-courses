Hello!!

You asked me for a 1 month free course on the things you need to
know about Ruby. This is the first of your 8 emails. If I am not
creating value for you with these emails, you can unsubscribe
with 1 click at the end of this email.

I'll let you in on a secret: Ruby is frustrating to install. If
you hand me a shiny new Mac laptop (macbook air, retina please),
I'd have to spend at least a couple of hours getting a ruby
version manager installed, and maybe another hour to become
productive. That's a pretty big investment just to try out some
code to see if you even LIKE Ruby, right?

It doesn't have to be this way; you can, within 2 minutes, have a
development environment up to play around with. Then, if things
go swimmingly, you can use one of the ruby installers I'll
describe and have things locally.

------------------------------------------------
The Secret 2 minute journey to Ruby Productivity
------------------------------------------------

Step 1: go to http://nitrous.io

Step 2: Sign in with GitHub

Step 3: Fire up a box and start coding

Unsure what to code? Here's a free walkthrough on Ruby in 100
Minutes ( http://tutorials.jumpstartlab.com/projects/ruby_in_100_minutes.html ) from the friendly Jumpstart Labs.

I'm not affiliated with Nitrous -- and the link isn't even an
affiliate link. I personally use Nitrous when teaching classes,
workshops, and RailsGirls. The boxes are free to get started, and
are powerful enough to develop on. Totes awesome.

You can also try out RubyFiddle (I wrote this) to sing 'n bottles
on the wall' ( http://rubyfiddle.com/riddles/8bda7/31 )

The easy win here: don't waste time installing Ruby locally to
find out if you like it. Instead, spend time having fun and
learning ruby instead!

---------------------------------
When you're ready to install Ruby
---------------------------------

You've tried it out, and Ruby is for you. You've heard people
tell you about Ruby installers, and maybe about homebrew. Here's
the decision tree you should use to figure out which you should
use:

If you have a mac

Comfortable with the command line? I recommend you look at rbenv
( https://github.com/sstephenson/rbenv ) to get started with
Ruby. If you have trouble getting rbenv to work, you should look
into rvm ( http://rvm.io ). Me? I use chruby and love it.

Not a command line guru? Don't worry, you will be soon enough.
But in the mean time, check out rvm, or the Rails Installer ( http://railsinstaller.org ), which has both Mac and Windows
varieties

If you use Windows

Use Rails Installer ( http://railsinstaller.org ) -- it is
seriously good and will get you running with Ruby, Git, Rails,
SQLite, and connect to SQL Server.

If you use Linux

You probably don't want my recommendations, but I like chruby ( https://github.com/postmodern/chruby ) and so will you.

----------------------------------------
Why use a ruby "version" manager at all?
----------------------------------------

Ruby is released quite often. In the last two years, we've seen
1.9.3, 2.0.0, and right now we are using 2.2.2. It's more common
than ever to switch back and forth to the Java compatible version
of Ruby JRuby. You'll probably have multiple projects, which were
written at different times in the space time continuum. You'll
want to run the Rails 3.2 in ruby 1.9.3, and new projects in Ruby
2.0.0, and try out new stuff in 2.1.

That will come naturally -- and it will be something you'll
experience. Some code written in "Ruby 1.9" (which could be 1.9.2
or 1.9.3) won't run in Ruby 1.8.7.

Thanks for reading the above. I'm going to come back in a few
days with a lesson on The cryptic craft of deploying Ruby
applications. If you have questions about this, hit reply and
I'll get back to you today.

- jesse
