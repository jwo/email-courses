Hi there! This is email number 7 of 8 in the 'What you need to
know about Ruby' email course you signed up for on
RubyOffRails.com. If I am not creating value for you with these
emails, you can unsubscribe with 1 click at the end of this
email.

By now, you've likely seen the terms RSpec and TestUnit and
MiniTest, and have trouble telling them apart. In Ruby Off Rails,
you'll see all three versions, and will be able to use any of
them depending on the project at hand.

RSpec
-----

A test framework that enables you to write expressive tests. The
"Spec" in RSpec stands for Specifications. The idea is to specify
how the program should behave. In the end, well written RSpec
reads like english.

<span class="n">it</span> <span class="s2">"calculates half-life
of 25"</span> <span class="k">do</span>
<span class="n">calc_half_life</span><span
class="p">(</span><span class="no">THE_THING</span><span
class="p">)</span><span class="o">.</span><span
class="n">should</span> <span class="n">eq</span><span
class="p">(</span><span class="mi">25</span><span
class="p">)</span>
<span class="k">end</span>

Newer versions of RSpec favor this method:

<span class="n">expect</span><span class="p">(</span><span
class="n">calc_half_life</span><span class="p">(</span><span
class="no">THE_THING</span><span class="p">))</span><span
class="o">.</span><span class="n">to</span> <span
class="n">eq</span><span class="p">(</span><span
class="mi">25</span><span class="p">)</span>

TestUnit
--------

TestUnit itself was in Ruby until version 1.8.7, and today is
generally used to refer to the Rails test suite. TestUnit was
replaced with MiniTest in Ruby 1.9, and Rails switched to
MiniTest in Rails 4.0.

MiniTest
--------

MiniTest is included with Ruby 1.9, and is an "assert" based
framework. This means it looks much like NUnit, JUnit, or the
other Unit based testing system:

<span class="n">assert_equal</span> <span
class="mi">5</span><span class="p">,</span> <span
class="n">calculated_value</span>

MiniTest/Spec is a specification based subsystem with minitest,
and allows you to write rspec like tests.

<span class="n">it</span> <span class="s">"calculates half-life
of 25"</span> <span class="k">do</span>
<span class="n">calc_half_life</span><span
class="p">(</span><span class="n">THE_THING</span><span
class="p">).</span><span class="n">must_equal</span> <span
class="mi">25</span>
<span class="n">end</span>

How do you choose between MiniTest and RSpec? Try each out, get
proficient in both, and then use the one that matches your brain
the closest. I used to <3 RSpec, and am now a MiniTest fan.

- jesse
