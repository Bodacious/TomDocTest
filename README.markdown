# The problem

To reproduce this error: 

    $ tomdoc some_ruby_file.rb
    
This give the following error:

      /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/tomdoc.rb:124:in `block in tomdoc': bad value for range (ArgumentError)
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/tomdoc.rb:120:in `map'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/tomdoc.rb:120:in `tomdoc'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/tomdoc.rb:257:in `parse'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/tomdoc.rb:56:in `initialize'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/scope.rb:19:in `new'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/scope.rb:19:in `tomdoc'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/generators/console.rb:9:in `write_scope_header'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/generator.rb:51:in `write_scope'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/generator.rb:41:in `block in process'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/generator.rb:40:in `each'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/generator.rb:40:in `process'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/generator.rb:34:in `generate'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/cli.rb:101:in `block (2 levels) in <class:CLI>'
      from /Users/Gavin/.rvm/rubies/ruby-1.9.3-p0-perf/lib/ruby/1.9.1/optparse.rb:1412:in `call'
      from /Users/Gavin/.rvm/rubies/ruby-1.9.3-p0-perf/lib/ruby/1.9.1/optparse.rb:1412:in `block in parse_in_order'
      from /Users/Gavin/.rvm/rubies/ruby-1.9.3-p0-perf/lib/ruby/1.9.1/optparse.rb:648:in `search'
      from /Users/Gavin/.rvm/rubies/ruby-1.9.3-p0-perf/lib/ruby/1.9.1/optparse.rb:1510:in `block in visit'
      from /Users/Gavin/.rvm/rubies/ruby-1.9.3-p0-perf/lib/ruby/1.9.1/optparse.rb:1509:in `reverse_each'
      from /Users/Gavin/.rvm/rubies/ruby-1.9.3-p0-perf/lib/ruby/1.9.1/optparse.rb:1509:in `visit'
      from /Users/Gavin/.rvm/rubies/ruby-1.9.3-p0-perf/lib/ruby/1.9.1/optparse.rb:1412:in `parse_in_order'
      from /Users/Gavin/.rvm/rubies/ruby-1.9.3-p0-perf/lib/ruby/1.9.1/optparse.rb:1341:in `order!'
      from /Users/Gavin/.rvm/rubies/ruby-1.9.3-p0-perf/lib/ruby/1.9.1/optparse.rb:1432:in `permute!'
      from /Users/Gavin/.rvm/rubies/ruby-1.9.3-p0-perf/lib/ruby/1.9.1/optparse.rb:1453:in `parse!'
      from /Users/Gavin/.rvm/rubies/ruby-1.9.3-p0-perf/lib/ruby/1.9.1/optparse.rb:1443:in `parse'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/cli.rb:118:in `parse_options'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/cli.rb:114:in `parse_options'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/lib/tomdoc/cli.rb:146:in `<top (required)>'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/gems/tomdoc-0.2.4/bin/tomdoc:7:in `<top (required)>'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/bin/tomdoc:19:in `load'
      from /Users/Gavin/.rvm/gems/ruby-1.9.3-p0-perf/bin/tomdoc:19:in `<main>'
