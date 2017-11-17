Hi there! This is email number 3 of 8 in the 'What you need to
know about Ruby' email course you signed up for on
RubyOffRails.com. If I am not creating value for you with these
emails, you can unsubscribe with 1 click at the end of this
email.

One of the examples you see showcasing Ruby awesomeness is the
ability to check if an object is blank? --- meaning you can check
the same object if it is nil (nothing), empty string (""), or an
empty array ([]) in one call.

empty_string = ""
empty_string.blank?
=> true
empty_array = []
empty_array.blank? => true
nothing = nil
nothing.blank?
=> true

The trouble is, if you open irb (or use RubyFiddle) to try this
out, you'll get a "NoMethodError". Very frustrating!

This method, "blank?", is added into Ruby by the Rails gem
ActiveSupport. To get this to work, you'll need to install the
gem, require it, and then you'll get the magical methods.

> gem install active_support

> irb

require 'active_support/all'

[].blank?

=> true

This raises an interesting question -- where does all this Ruby
code come from? Let's explore.

---------
Ruby Core
---------

The Ruby language comes with many modules -- after all, if you
wanted a language with no libraries, you'd have picked up LISP.
OK, so what comes with Ruby?

Things like Enumerable, String, Number, and most of the code
you'll use daily. This code is in "Ruby Core", and each method
and class is available to you without having to 'require' it.

To see example usage, and read the documentation, check out:

* How to open, read, or write to a file:
http://ruby-doc.org/core-2.0.0/File.html ( http://ruby-doc.org/core-2.0.0/File.html )

* The super awesome things Enumerable gives you:
http://ruby-doc.org/core-2.0.0/Enumerable.html ( http://ruby-doc.org/core-2.0.0/Enumerable.html )

----------------
Standard library
----------------

The second set of code each Ruby install has is the "Ruby
Standard Library". The standard lib has code for special
purposes, and can do everything from parse CSV files to create
XML/RSS, and server webpages.

The standard library contains well tested code that most people
reach for Gems for. Pro Tip: learning the standard library is the
single greatest thing you can do to take a leap from good to
great.

Examples from the Standard Library:

* Parse CSV Files -
http://ruby-doc.org/stdlib-2.0.0/libdoc/csv/rdoc/CSV.html ( http://ruby-doc.org/stdlib-2.0.0/libdoc/csv/rdoc/CSV.html )

* Parse JSON -
http://ruby-doc.org/stdlib-2.0.0/libdoc/json/rdoc/JSON.html#method-i-parse
( http://ruby-doc.org/stdlib-2.0.0/libdoc/json/rdoc/JSON.html#method-i-parse )

* Test your code with MiniTest -
http://ruby-doc.org/stdlib-2.0.0/libdoc/minitest/rdoc/index.html
( http://ruby-doc.org/stdlib-2.0.0/libdoc/minitest/rdoc/index.html )

* Host a website with no dependencies:
http://tobyho.com/2009/09/16/http-server-in-5-lines-with/ ( http://tobyho.com/2009/09/16/http-server-in-5-lines-with/ )

--------
RubyGems
--------

Gems are reusable libraries of code, distributed in an easily
consumable manner. They can do everything from host your site
(unicorn), to a full framework (rails), to handle money
calculations.

By far, Gems are the secret sauce of productivity in Ruby and
Rails applications. Developers bring in a Gem and instantly have
a way to upload images, scale and size them, and store them in
S3. Or a way to test your entire web stack with a real browser
(capybara). Or use an entirely different test suite (rspec).

The canonical way to install gems is to use Bundler. You run:

'gem install bundler'

And then create a Gemfile. (sample Gemfile from a RubyOffRails
project). The Gemfile specifies which gems you'd like to install,
and a version if necessary.

To install the gems:

'bundle install'

And the gems are downloaded, along with every dependency those
gems need. The power of this cannot be understated -- instead of
a list of 20 other libraries to install, you install 1.

The best place to find a gem for a particular task is RubyToolbox
( https://www.ruby-toolbox.com/ ). You can browse by topic, and
(importantly), see if the gem is active or not by seeing the last
commit date. ProTip: don't install gems that appear abandoned.

We've taught you how to get started, how to deploy Ruby, and how
to actually use Ruby code. I know you have many things to do with
your day than just learning Ruby; so: consider taking Ruby Off
Rails. You'll get advice like this and hours of videos distilled
into how to be productive as a Ruby Developer.

- jesse
