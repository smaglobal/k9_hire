<img width="1673" alt="k1" src="https://user-images.githubusercontent.com/35616113/208560691-a2068cef-60e8-43ed-b390-0474235389b6.png">

# K9 Hire

A Web App implemented in Ruby on Rails as a project during Le Wagon.

## Description

Hiring dogs couldn't get easier. A user friendly application that lets users hire dogs around their location using live search feature.

## Getting Started

## Install

### Clone the repository

```shell
git clone git@github.com:smaglobal/k9_hire.git
cd project
```

### Check your Ruby version

```shell
ruby -v
```

The ouput should start with something like `ruby 3.0.3`

If not, install the right ruby version using [rbenv](https://github.com/rbenv/rbenv) (it could take a while):

```shell
rbenv install 3.0.3
```

### Install dependencies

Using [Bundler](https://github.com/bundler/bundler) and [Yarn](https://github.com/yarnpkg/yarn):

```shell
bundle && yarn
```

### Set environment variables

* Any sensitive data such as API keys can be set up in .env file e.g. (**process.env.STRIPE_SECRET_KEY)
* Require Stripe, Mapbox and Cloudinary APIs keys

### Initialize the database

```shell
rails db:create db:migrate db:seed
```

### Add heroku remotes (Optional)

Using [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli):

```shell
heroku git:remote -a project
heroku git:remote --remote heroku-staging -a project-staging
```

## Serve

```shell
rails s
```

## Deploy 

### With Heroku pipeline (recommended)

Push to Heroku staging remote:

```shell
git push heroku-staging
```

Go to the Heroku Dashboard and [promote the app to production](https://devcenter.heroku.com/articles/pipelines) or use Heroku CLI:

```shell
heroku pipelines:promote -a project-staging
```

### Directly to production (not recommended)

Push to Heroku production remote:

```shell
git push heroku
```
