# Blogging App

This is will be a Ruby on Rails Blogging Application. It's designed to see how you'd perform in real world work. I don't care if you can code a binary tree in Ruby. I care that you can write performant Rails applications using best practices and following The Rails Way. Read this entire page before getting started. Attention to detail is extremely important. Even if you're applying at the Junior level, getting details right is extremely important.

## Background

Create a Rails application using the following technology

1. Ruby 3.02
2. Rails 6.1.4.1
3. Hotwire, specifically the Turbo + Stimulus frameworks.
4. PostgreSQL
5. NO Rspec. Use the standard Rails testing paradigm (MiniTest) presented on this page: https://guides.rubyonrails.org/testing.html. Use fixtures where appropriate, but if you must have object creation, use the Fabrication gem (not FactoryBot.)
6. Model, System, Functional, Integration, and Views should be tested. If you have Jobs, Helpers, or Mailers, those should be tested.
7. No external javascript frameworks beyond Hotwire/Turbo/Stimulus
8. For Senior candidates, use Russian Doll and low level caching where appropriate: https://guides.rubyonrails.org/caching_with_rails.html, use Memcache
9. There should be a Procfile for the application -> https://devcenter.heroku.com/articles/procfile and Foreman should work to start your app and all the relevant processes -> https://github.com/ddollar/foreman
10. Use Tailwind for styling -> https://tailwindcss.com and https://github.com/rails/tailwindcss-rails
11. Minimal is the key. Simplicity. White background. Big, readable text. -> https://uxmovement.com/content/why-you-should-never-use-pure-black-for-text-or-backgrounds/
12. Must be localized. For now, the languge should be English, but we want to be able to easily add more languages using a .yml file. (this means your code should have localizable strings and en.yml should translate those strings. -> https://guides.rubyonrails.org/i18n.html
13. Use Action Text as necessary -> https://edgeguides.rubyonrails.org/action_text_overview.html
14. Use Active Storage if necessary
15. Consider using Decent Exposure -> https://github.com/hashrocket/decent_exposure
16. Create a seed file to populate your application with sample data. Use Faker. https://github.com/faker-ruby/faker

## Requirements

1. As a person who wants to write a blog, I want to sign up for an account to create and manage a blog
2. I need to be able to sign in, sign out, and update my email address and password
3. I want to write a blog post and edit the following metadata -- Title, Publish Date, Draft Status
4. I want a non-logged in user to be able to read my blog posts and the blog posts of other users
5. I want to be able to edit or delete posts

### For Senior Candidates
6. Add the option to create/edit/delete a main image for blog posts
7. Add tagging for blog posts using acts-as-taggable-on -> https://github.com/mbleigh/acts-as-taggable-on

### Bonus Points
Using a free account from Algolia, implement a full text, tag, and author search on the public blog index page.

## Delivery

Send a link to the github repository for your code to brian@icouch.me and cc:ing matt@icouch.me
Deploy to Heroku and provide a URL to your running application (use only free/hobby resources on Heroku) and include the link to your application in your README

## How you'll be evaluated

1. Quality of testing. Tests should run quickly and comprehensively test the application
2. Clean and well-organized code, DRY. https://thoughtbot.com/blog/sandi-metz-rules-for-developers
3. Following of instructions

## Why are you doing this?

This test represents some level of real world application development. This is the kind of day-to-day thinking and working you'd do on the team. There's a requirement to be able to read websites, study a technology/gem/tool and be able to apply that knowledge. I'm most interested if you have the ability to learn and apply, while following good testing practices. I know this is hard work, but the intent is that it should be fun as well, perhaps exposing you to some different ideas that you might not have used before.
