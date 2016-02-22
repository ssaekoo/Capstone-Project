# offTheBeatenTrack

GoodTreks is a web application inspired by GoodTreks built using Ruby on Rails and React.js. GoodTreks allows users to:

##MVP:
- [ ] Create an account
- [ ] Log In/Log out
- [ ] Create, read, and edit a trek
- [ ] Users can review on their experience of the trek
- [ ] Users can rate difficulty of trek
- [ ] Users can endorse special equipment necessary for the trek

###Extras:
- [ ] Tags
- [ ] Users can sort via region and difficulty and tags

## Design Docs
* [View Wireframes][views]
* [React Components][components]
* [Flux Stores][stores]
* [API endpoints][api-endpoints]
* [DB schema][schema]

[views]: ./docs/GoodTreks.png
[components]: ./docs/ComponentHierarchy.md
[stores]: ./docs/FluxStores.md
[api-endpoints]: ./docs/APIEndpoints.md
[schema]: ./docs/schema.md

## Implementation Timeline

### Phase 1: Backend setup, Treks Model, and User Authentication (0.5 days)

**Objective:** Functioning rails project with Authentication

- [ ] create new project
- [ ] create `User` model
- [ ] authentication
- [ ] user signup/signin pages
- [ ] blank landing page after signin
- [ ] create `Trek` model

### Phase 2: API, and basic APIUtil ( 1 days)

**Objective:** Treks can be created, read, edited and destroyed through
the API.

- [ ] seed the database
- [ ] CRUD API for Treks (`TreksController`)
- [ ] jBuilder views for Treks
- [ ] setup Webpack & Flux scaffold
- [ ] setup `APIUtil` to interact with the API
- [ ] test out API interaction in the console.

### Phase 3: Flux Architecture and Router (1.5 days)

**Objective:** Treks can be created, read, edited and destroyed with the
user interface.

- [ ] setup the flux loop with skeleton files
- [ ] setup React Router
- implement each Trek component, building out the flux loop as needed.
  - [ ] `TreksIndex`
  - [ ] `TrekDetail`
  - [ ] `TrekForm`
- [ ] save Treks to the DB when the form loses focus or is left idle
  after editing.

### Phase 4: Start Styling (1 days)

**Objective:** Existing pages (including singup/signin) will look good.

- [ ] create a basic style guide
- [ ] position elements on the page
- [ ] add basic colors & styles

### Phase 5: Location (1 day)

**Objective:** Treks belong to a location, and can be viewed by location.

- [ ] create `Trekbook` model
- build out API, Flux loop, and components for:
  - [ ] Trekbook CRUD
  - [ ] adding Treks requires a Trekbook
  - [ ] moving Treks to a different Trekbook
  - [ ] viewing Treks by Trekbook
- Use CSS to style new views

Phase 3 adds organization to the Treks. Treks belong to a Trekbook,
which has its own `Index` view.

### Phase 6: Tags (1.5 days)

**Objective:** Treks can be tagged with multiple tags, and tags are searchable.

- [ ] create `Tag` model and join table
- build out API, Flux loop, and components for:
  - [ ] fetching tags for Treks
  - [ ] adding tags to Treks
  - [ ] creating tags while adding to Trek
  - [ ] searching Trek by tag
- [ ] Style new elements

### Phase 7: Allow Complex Styling in Treks (1.5 days)

**objective:** Enable complex styling of Treks.

- [ ] Integrate `react-quill` (based on Quill.js).
- [ ] Use Rails helpers to sanitize HTML before rendering.
- [ ] Style the new Quill elements.

### Phase 8: Styling Cleanup and Seeding (1 day)

**objective:** Make the site feel more cohesive and awesome.

- [ ] Get feedback on my UI from others
- [ ] Refactor HTML classes & CSS rules
- [ ] Add modals, transitions, and other styling flourishes.

### Bonus Features (TBD)
- [ ] Search through Treks for blocks of text
- [ ] Pagination / infinite scroll for Treks Index
- [ ] Google map for Treks
- [ ] Changelogs for Treks
- [ ] Equipment recommendations for Trek
- [ ] Backpackers dictionary

[phase-one]: ./docs/phases/phase1.md
[phase-two]: ./docs/phases/phase2.md
[phase-three]: ./docs/phases/phase3.md
[phase-four]: ./docs/phases/phase4.md
[phase-five]: ./docs/phases/phase5.md