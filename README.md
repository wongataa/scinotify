# SciNotify
A project to create an alerts/ a daily email for relevant clinical trials by interacting with the open source [US clinical trials database](https://clinicaltrials.gov/). [Here's the API](https://clinicaltrials.gov/api/gui).

# Features

## Cornerstone Feature
 * Collect the user's email address
 * Allow the user to save a list of keywords
 * Every day, search the US clinical trial database for trials that match the keywords
 * When a new trial or trials appear email these to the user

## Other Features
 * Allow the user to save links to papers
 * Autopopulate with links to new papers from a user's keywords
 * Email the user one random paper a day from their saved (and unread) links
 * Create a chrome extension to save a link offsite via a button or keyboard shortcut

### Resources for building a Chrome extension
[Zotero](https://www.zotero.org/support/dev/start) is an open source citation manager that has similar functionality

# Get Started
This project uses PHP Laravel (and a Postgres DB). A local development env is easily set up using docker & [Laravel Sail](https://laravel.com/docs/8.x/sail). Do `composer install` then `sail up -d` to bring up the services listed in the docker-compose file. See the .env file for using XDEBUG

