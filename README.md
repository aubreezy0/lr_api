# Magic Lunch Ball - API

Magic Lunch Ball is a redux (and then some) of an original project for class, called "Lunchbx." I'm refactoring the site to add a Google Maps API. User will click on a magic eight ball, which will offer a local restaurant recommendation with related map.

I am building on the original Lunchbx database, which allowed users to enter their own restaurants. V3 will capitalize on that by allowing users to log in and save their restaurant results.

I am keeping (most) of the original README content from the original concept. It demonstrates the mothodologies used (including ERDs, etc.) that demostrate an understanding of the process of feature development.

In the meantime you can follow along at:
<ul>
<li>https://github.com/aubreezy0/lr_client and</li>
<li>https://github.com/aubreezy0/lr_api</li>
</ul>

Thank you!

# README from V1 iteration, "Lunchbx" (Not Magic Lunch Ball)

## Repos:
<ul>
<li>Front End: https://github.com/aubreezy0/lunchbx-client</li>
<li>Back End: https://github.com/aubreezy0/lunchbx-api</li>
<li>Deployed Client: https://aubreezy0.github.io/lunchbx-client</li>
<li> Deployed API: https://calm-journey-36314.herokuapp.com/</li>
</ul>

## Process
I started with setting up the initial Rails Server. I added one resource, a Restaurant table that would have user_id (from the existing user table) as a foreign key. I created new CURL scripts for the restaurant CRUD functions. I then built very basic forms in the front end to begin testing the API calls. I was stuck for quite some time on Add Restaurant. In a classic bit of syntactic drama, the problem came down to missing an “s” in Headers in the API call. Once fixed all sides were happily chatting and I moved on to the front end user experience.

## ERDs:
My initial ERD was for a many-to-many relationship, however my final ERD draft</a> had a one to many relationship, one user to many restaurants.

<img src="https://i.imgur.com/pw2EkdV.png">

## Future Development
In the next iteration of Lunchbx I will be adding additional resources for neighborhoods and teams, giving users the ability to put together their own groups for sharing and saving restaurants. I will also be exploring tying in the Four Square API.

## Technologies Used
Ruby on Rails

## API Routes and Methods

<img src="https://i.imgur.com/ky6iYhZ.png">

## How do I play?

#### Easy as 1, 2, 3:

<ol>
<li>Fork and clone this repo and the <a href="https://github.com/aubreezy0/lunchbx-client" target="_blank">front end repo</a></li>
<li>Run `brew install heroku` for icu4c, node dependencies</li>
<li>Run `bin/rails server`. Check out localhost:4741. If you see "Yay, you're on Rails!" You're good to go!</li>
</ol>
