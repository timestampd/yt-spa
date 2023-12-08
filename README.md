# YouTube Video Browser

## Requirements

- [x] Search form: preview youtube cover image
- [x] On search, search results page  (https://developers.google.com/youtube/v3/docs/search)
  - [x] Sort results by date, rating, relevance
  - [x] Title links to video on YouTube
  - [x] Thumbnail
  - [x] Description
  - [x] Display total number of comments on each video
- [x] Use developer app credentials so sign-in is not required?
- [ ] Dev/prod setups

I started with ideas from https://codepen.io/jorgebucaran/pen/ZeByKv, https://github.com/loteoo/hyperapp-starter. Then I scrapped those projects and worked in a more wild west approach to explore the basics of Web Components instead of the shades of different frameworks.

### Extension Ideas

- Better presentation for different loading states
- Pagination
- Compression/separation/CI/CD
- Testing
- More explicit error handling
- Keyboard shortcuts
- Embedded video player instead of redirect to YouTube for playback
- Login
  - Use YouTube API library (`<script src="https://apis.google.com/js/api.js"></script>`)
  - Interact with video (Like, Comment)
  - Playlist management


## Components

- Search page
- Search input
- Video item


## Setup

1. Retrieve a Google API key from https://console.cloud.google.com/apis/credentials.
1. Copy `config-example.js` to `config.js` and update the `GOOGLE_API_KEY` in it.
1. Open `app.html` in a browser.

By default, a project's YouTube Data API quota is 10,000 units per day, and each Search call uses 100 units.


## Original Prompt

```
Exercise details:

The YouTube Data API (https://developers.google.com/youtube/v3/docs/) provides access to YouTube. In this assignment you will write a single-page web application which uses the YouTube data api to provide a user interface for search. Please use Web Components. We use Lit but you can use any Web Component library or none at all. If you choose to use code generators or a boilerplate project as a starting point, please make sure we can tell which parts of the project are yours and which are generated or from the boilerplate. Descriptions in the readme and a range of commits helps with this.

Your application should consist of a Search view that contains the following features:

·  Search by keyword
·  Sort results by date, rating and relevance
·  List view of results should contain:
	o Title that is a link that opens the video on YouTube.com
	o Thumbnail
	o Description
	o Display total number of comments on each video.

Try not to get bogged down with the look and feel of the application - we’re more interested in how you organize the project and which tools (patterns, libraries, dependency management, etc.) you choose to use. This should be production ready when done and appear like any other feature you would work on for a product.

When you're finished, please put your project in a repository on Github and send us a link. We will then do a pair programming session where we'll have some questions for you about your code and possibly make some additions to it.
```
