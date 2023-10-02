
## prerequisite: install Git, ruby, bundle, webrick


1. jekyll is based on Ruby.
    RubyGem is equivalent to NPM of Node.js 
        gem install jekyll

        gem install bundle

2.  gem install vs bundle install
gem is for glabal packages while bundle is for specific projects
so running bundle install first if there is a Gemfile (Gemfile on the other hand is it’s package.json)


 3. Make sure the version is corrrect: 
        My version:

        ruby -v  3.2.2

        gem —version 3.4.19




4. A issue: When running: 

        bundle exec jekyll serve   (Start to serve the jekyll website)

    this error come out :
        
        cannot load such file -- webrick****

    That’s because  Ruby 3.0 version up does not come with Webrick(Ruby’s http server),

    so you will need to install first:

        gem install webricks

    Then add it to the project:

        bundle add webrick

    Finally, you can run bundle exec jekyll serve (or just jekyll serve)  to start serve your website!