# Heroku Buildpack for database.examole.yml

Heroku buildpack for setting up databes.yml from database.example.yml

# Usage

## Add a detect hook (required)

In order for this buildpack to execute, it will look for a `database.example.yml` file in your app's config.

## Add Buildpack

### Setup using heroku's native support for multiple buildpacks

Heroku natively also support's multiple buildpacks, the same setup as above can be achieved as follows:

    heroku buildpacks:clear
    heroku buildpacks:set heroku/ruby
    heroku buildpacks:add --index 1 https://github.com/s33m4nn/database-yml-buildpack

# Configuration

todo