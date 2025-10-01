# Hello Rails Movies

This Rails application is the "Hello Rails" starter used in CHIPS. It exposes a basic CRUD interface for movies so you can practice working with controllers, views, and the Active Record ORM.

## Prerequisites

- Ruby 3.3.8 (match the version pinned in `Gemfile`)
- Bundler (`gem install bundler` if you don't already have it)
- SQLite 3 (for the development and test databases)

## Getting Started

1. Install gems: `bundle install`
2. Set up the database (creates, migrates, and seeds): `bin/rails db:setup`
3. Start the server: `bin/rails server`
4. Visit `http://localhost:3000/movies` to browse, create, update, or delete movie records.

If you change your schema later, rerun `bin/rails db:migrate`. To reseed demo data, use `bin/rails db:seed`.

## Running the Test Suite

Execute `bin/rails test` to run the Rails test suite. Add feature or model tests as you build out more functionality.

## Project Structure Highlights

- `app/controllers/movies_controller.rb` implements the RESTful actions for movies.
- `app/views/movies/` contains the ERB templates for the CRUD UI.
- `db/seeds.rb` loads sample movie data inspired by RottenPotatoes.

## Useful Commands

- `bin/rails console` launches an interactive console backed by the Rails environment.
- `bin/rails routes` lists the available routes; the scaffold defines the standard REST paths for movies.
- `bin/dev` runs the dev server with concurrent Rails and JS processes (if you have foreman installed).

Refer to the official [Rails Guides](https://guides.rubyonrails.org/) for deeper explanations of the framework components used here.
