massdebate
==========

(TODO: link to heroku app)

As much as I love to work on massdebate alone, I happily accept pull requests.

What?
-----
This is a simple web app, that tries to encourage good debate though the user interface.  It is meant to be easy for visitors to oject to specific points in a transparent way. All critisism branches must be dealt with for an argument to be conidered correct.

History
-------
This was a idea I had years ago, and now that I have some freetime I figure why not try it out again.

Why python django?
------------------
I've been wanting to learn python for a wile now.  So that's why the code might be awkward in places.  Also I figured that I'd get more pull requests in django then if I had written it in an experimental nightly build of scala.

How to set up a heroku instance
-------------------------------
(please god there has to be a better way)

(create a heroku acount, possibly have to deal with permisioning/ssh bs)

```bash
$ heroku login
$ git clone https://github.com/marklemay/massdebate.git
$ cd massdebate/
$ heroku create
$ git push heroku master
$ heroku run python manage.py syncdb
$ heroku open
```

