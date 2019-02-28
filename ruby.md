# Ruby Cheatsheet

## Fix gem pristine warning msgs

Clear rvm cache
`rm -rf ~/.rvm/gems/ruby-2.5.3@global/cache`

After that I redid the following:

`gem pristine --all`
`bundle install`
`bundle exec spring binstub --all`

## Fix file system permission issue with rubygems

Replace with current ruby version in use on system:
`sudo chown -R $(whoami) ~/.rmv/rubies/ruby-2.5.3/lib/ruby/gems/2.5.0/gems`

