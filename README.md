Static Build Pack
========================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpack) for static websites, or whatever you want.

Use
-------

    $ ls
    index.html      somedir/
    $ git init
    $ heroku create --stack cedar --buildpack https://github.com/pearkes/heroku-buildpack-static
    $ git add .
    $ git commit -m "initial commit"
    $ git push heroku master

Optional Configuration
-------
The Apache configuration file is located in `conf/httpd.conf`. To customize, fork and use your fork as the buildpack url on app create.

Improving
-------

To test changes to this buildpack, fork it on Github. Push up changes to your fork, then create a test app with --buildpack <your-github-url> and push to it.

All improvements are appreciated!

License
-------

Copyright (c) 2012 Jack Pearkes

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
