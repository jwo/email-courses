Hi there! This is email number 6 of 8 in the 'What you need to
know about Ruby' email course you signed up for on
RubyOffRails.com. If I am not creating value for you with these
emails, you can unsubscribe with 1 click at the end of this
email.

Have you heard of JRuby? Or the term 'MRI'? Or Rubinius? Chances
are, you have not --- I hadn't until a year into my Ruby career.
But each have unique qualities and are right in certain
scenarios.

--------------------
First, what is "MRI"
--------------------

To many, 'MRI' is Ruby -- it stands for "Matz's Ruby
Implementation", and is the standard version of Ruby. It's
written in C, and is the only version that the Ruby founder Matz
works on.

When Ruby "2.0" is released, that means MRI. Sometimes, people
call it "c-ruby", but it's all the same thing. ProTip: If someone
is talking about Ruby, it's MRI. If it's something else, they'll
let you know.

-----
JRuby
-----

The J in JRuby standard for Java; JRuby runs on the JVM (java
virtual machine), and can interface and run any language on the
JVM (like Java or Clojure). JRuby's main benefit is the JVM,
which means it can take full advantage of millions of dollars of
investments making the JVM run in parallel and on Windows, Unix,
and Linux machines.

With JRuby, you can use more than one core on your machine
(multi-threading). Right now, MRI cannot do CPU intensive
multi-threading. JRuby also runs nearly all Ruby code and Gems --
the exception being any c-extensions (calling out to pure
c-code), and any UNIX specific commands like Forking.

But, JRuby is making a huge resurgence, and is definitely a
project to watch and take part of. With the Ruby version
managers, using JRuby is the same as switching to version 1.9.3
-- very exciting times! It's also very easy to run JRuby on
Heroku ( https://blog.heroku.com/archives/2012/12/13/run_jruby_on_heroku_right_now ).

--------
Rubinius
--------

Rubinius started as a way to write Ruby in Ruby (since MRI is
written in C). It ended up as a powerful virtual machine with
fast garbage collection and multi-threaded capabilities that
rival JRuby.

Rubinius announced in its version 2.0 launch that it would focus
on writing fast, concurrent web applications. This focus could
make Rubinius THE variety to use when creating APIs that need to
be 10ms-50ms fast.

-----------------------
So What Should You Use?
-----------------------

As you're learning Ruby, you should use MRI -- it's the most
widely accepted and the default installation across the web. When
you encounter a project that needs multi-threaded awesomeness,
try out both JRuby and Rubinius and see which you like better.

Have you heard of either JRuby or Rubinius before? I'd love to
hear from you -- hit reply and let me know!

- jesse
