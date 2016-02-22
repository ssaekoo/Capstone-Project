API Endpoints
HTML API

Users

GET /users/new
POST /users
PATCH /users

Session
GET /session/new
POST /session
DELETE /session

JSON API

Treks

GET /api/treks
	Treks index/search
	accepts tag_name query param to list treks by tag
POST /api/treks
GET /api/treks/:id
PATCH /api/treks/:id
DELETE /api/treks/:id

Tags

GET /api/tags
includes query param for typeahead suggestions
POST /api/treks/:trek_id/tags: add tag to trek by name
DELETE /api/treks/:trek_id/tags/:tag_name: remove tag from trek by if user_count hits 0