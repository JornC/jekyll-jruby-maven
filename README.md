# Jekyll with JRuby and Maven

Jekyll runs fine with JRuby and Maven, at least on Mac and Linux.

Run with:

`
mvn gem:exec@jekyll-serve
`

It works as expected on Mac and Linux, but not on Windows:
    
    [INFO] Configuration file: c:\Users\username\projects\jekyll-jruby-maven/src/main/resources/_config.yml
    [INFO] Source: c:\Users\username\projects\jekyll-jruby-maven/src/main/resources
    [INFO] Destination: c:\Users\username\projects\jekyll-jruby-maven\target\classes
    [INFO] Incremental build: disabled. Enable with --incremental
    [INFO] Generating...
    [INFO] C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/jekyll-3.0.2/lib/jekyll/utils.rb:117:in `open': Permission denied - c
    :/Users/username/projects/jekyll-jruby-maven/src/main/resources/css (Errno::EACCES)
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/jekyll-3.0.2/lib/jekyll/utils.rb:117:in `has_yaml_header?'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/jekyll-3.0.2/lib/jekyll/reader.rb:43:in `block in read_directories'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/jekyll-3.0.2/lib/jekyll/reader.rb:43:in `select'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/jekyll-3.0.2/lib/jekyll/reader.rb:43:in `read_directories'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/jekyll-3.0.2/lib/jekyll/reader.rb:17:in `read'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/jekyll-3.0.2/lib/jekyll/site.rb:144:in `read'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/jekyll-3.0.2/lib/jekyll/site.rb:57:in `process'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/jekyll-3.0.2/lib/jekyll/command.rb:28:in `process_site'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/jekyll-3.0.2/lib/jekyll/commands/build.rb:60:in `build'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/jekyll-3.0.2/lib/jekyll/commands/build.rb:35:in `process'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/jekyll-3.0.2/lib/jekyll/commands/build.rb:18:in `block in init_
    with_program'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/mercenary-0.3.5/lib/mercenary/command.rb:220:in `call'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/mercenary-0.3.5/lib/mercenary/command.rb:220:in `block in execute'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/mercenary-0.3.5/lib/mercenary/command.rb:220:in `each'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/mercenary-0.3.5/lib/mercenary/command.rb:220:in `execute'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/mercenary-0.3.5/lib/mercenary/program.rb:42:in `go'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/mercenary-0.3.5/lib/mercenary.rb:19:in `program'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/gems/jekyll-3.0.2/bin/jekyll:17:in `<top>'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/bin/jekyll:1:in `load'
    [INFO] from C:/Users/username/projects/jekyll-jruby-maven/target/rubygems/bin/jekyll:1:in `<top>'
    [INFO] from -e:1:in `load'
    [INFO] from -e:1:in `<top>'