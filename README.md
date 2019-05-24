# Public demo Eventmaker SSO

This app is an example of OAuth 2 client. It was built in order to test an Eventmaker provided SSO. It's based on [this demo app](https://github.com/doorkeeper-gem/doorkeeper-sinatra-client).


## Installation

You will need a working installation of ruby. First clone this repository, then install dependencies with `bundle install` (you will neeed bundler for that).

## Configuration

### Client application

### Environment variables

You need to setup few environment variables in order to make the client work. You can either set the variables in you environment:

```bash
export CLIENT_ID="129477f..."
export CLIENT_SECRET="c1eec90..."
export CLIENT_REDIRECT_URI="http://localhost:9393/callback"
export PROVIDER_URL="http://you-server-app.com"
```

or set them in a file named `.env` in the app's root. This file is loaded automatically by the app.

```
# .env
CLIENT_ID="129477f..."
CLIENT_SECRET="c1eec90..."
CLIENT_REDIRECT_URI="http://localhost:9393/callback"
PROVIDER_URL="http://you-server-app.com"
```

## Start the server

Fire up the server with: `bundle exec rackup config.ru`
