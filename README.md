# Heroku buildpack for meteor
Forked from https://github.com/jordansissel/heroku-buildpack-meteor

(Changed MongoDB hoster to MongoLab.)

## Usage

```
% heroku create --stack cedar --buildpack https://github.com/benzenwen/heroku-buildpack-meteor.git
```

## Example

Create a sample app with 'meteor'

```
% meteor create --example wordplay
wordplay: created.

To run your new app:
   cd wordplay
   meteor
```

Put it in git.

```
% cd wordplay
% git init
Initialized empty Git repository in /tmp/a/wordplay/.git/
% git add .
% git commit -m "Sample wordplay app!"
```

Create your heroku app

```
% heroku create --stack cedar --buildpack https://github.com/benzenwen/heroku-buildpack-meteor.git
```

Deploy it

```
% git push heroku
```

Enjoy!
