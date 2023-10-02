# Githubpages jekyll for personal blog website

My version:

ruby -v  3.2.2

gem —version 3.4.19

RubyGem is equivalent to NPM of Node.js 

Gemfile on the other hand is it’s package.json

When running 

bundle exec jekyll serve   (Start to serve the jekyll website)

this error come out :

****cannot load such file -- webrick****

That’s because  Ruby 3.0 version up does not come with Webrick(Ruby’s http server),

so you will need to install first:

gem install webricks

Then add it to the project:

bundle add webrick

Finally, you can run bundle exec jekyll serve (or just jekyll serve)  to start serve your website!