
This is my personal website.


## Run with Docker

`docker build . -t my_website`

`docker run -d -p 4000:4000 my_website`

Then can access the website at `localhost:4000`

## Run locally

Follow some of the instructions in the [github tutorial] (https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/)
but it is less complicated even.

To install necessary libs:

`gem install bundler`

`bundle install`


To run on localhost:4000 :
`bundle exec jekyll serve`
