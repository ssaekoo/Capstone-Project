##trekStore
- Actions:
	- receiveAlltreks
	- receiveSingletrek
	- removetrek

- Listeners:
	- treksIndex
	- trekDetail
	- trekFormStore

- trekFormStore
	- Actions:
		- receivetrekFormParams

	- Listeners:
		- trekForm
		- trekStore

- searchStore
	- Actions:
		- receiveSearchParams

	- Listeners:
		- SearchIndex

- searchSuggestionStore

	- Actions:
		- receiveSearchSuggestions
	- Listeners:
		- SearchSuggestions

##tagStore

	- Actions:
		- receiveAllTags
	- Listeners:
		- clickedTag
