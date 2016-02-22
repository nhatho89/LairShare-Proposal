# FresherNote

**NB:** This should be a link to your production site


## Minimum Viable Product

LairShare is a web application inspired by AirBnB built using Ruby on Rails, jQuery, AJAX
and React.js. LairShare allows supervillains who want to take a vacation, but don't want to
lose the supervillainy feel of their secret hideouts. Anominity is guaranteed!



General Functions

- [ ] Create an account
- [ ] Login / Logout
- [ ] Demo user login

Logged Out Functions

- [ ] Search function (locations, start and end dates)
- [ ] Render result with list and Google Maps
- [ ] Update local results display after map movement
- [ ] View listing details with ratings/comments from previous guests

Logged In Functions

- [ ] Submit booking request
- [ ] Submit rating and comment after the final stay date
- [ ] View profiles of other users

Host Functions

- [ ] Create new listings
- [ ] Edit current listings
- [ ] View profiles of requesters (level-2 details with reviews from other hosts)
- [ ] Approve/Deny booking request


Extra

- [ ] Drop down location suggestions on search bar
- [ ] Bouncing map icon
- [ ] Redirect link for non SF searches
- [ ] Highlights result display when hovering over map icon

## Design Docs
* [View Wireframes][views]
* [React Components][components]
* [Flux Stores][stores]
* [API endpoints][api-endpoints]
* [DB schema][schema]

[views]: ./docs/views.md
[components]: ./docs/components.md
[stores]: ./docs/stores.md
[api-endpoints]: ./docs/api-endpoints.md
[schema]: ./docs/schema.md

## Implementation Timeline



### Phase 1: User Authentication / JSON API (1 Day)

Backend Implementations:

- [ ] User model/controller and session controller
- [ ] User_profile model/controller
- [ ] Room model/controller
- [ ] JSON API
- [ ] Static Page controller
- [ ] Test Seed Data

### Phase 2: Flux Architecture (2 days)

Frontend Implementations:

- [ ] React view structure with Flux and React Router
- [ ] RoomStore with ApiUtil and RoomActions
- [ ] Home page
- [ ] Google Maps API
- [ ] Render search results on page
- [ ] Real time update while searching with map

### Phase 3: Room details and User profile pages (1.5 days)

Frontend Implementations:

- [ ] show page of a listed room with descriptions and pricing
- [ ] overlay image gallery
- [ ] user profile page

### Phase 4: Room ratings and reviews (2 day)

Backend Implementations:

- [ ] Reservation model/controller
- [ ] Feedback Star Rating model/controller

Frontend Implementations:

- [ ] reservation request in room's show page
- [ ] reservation summary in user account page
- [ ] cancellation buttons for future reservations
- [ ] review buttons for past reservations
- [ ] review form page
- [ ] add ratings and reviews to room show page

### Phase 5: Room listings (2 day)

Backend Implementations:

- [ ] improve room model/controller
- [ ] improve reservation model/controller
- [ ] improve users controller

Frontend Implementations:

- [ ] new listing form
- [ ] edit existing room form
- [ ] delete room or suspend reservation
- [ ] add room status/summary to host user's account page
- [ ] add reservation approval/denial functions
- [ ] hosts have ability to see more details of the requester


### Phase 6: Styling Cleanup and Seeding (.5 day)

Backend Implementations:

- [ ] create more seed data
- [ ] Don't allow visitors to alter data

Frontend Implementations:

- [ ] ensure style consistency
- [ ] add transition animations

Extra Features
- [ ] Drop down location suggestions on search bar
- [ ] Bouncing map icon
- [ ] Redirect link for non SF searches
- [ ] Highlights result display when hovering over map icon
