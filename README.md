# YouTube Video Browser

## Requirements

- [ ] Front page with prominent Search box, top header
- [ ] Search form: autocomplete, preview youtube cover image
- [ ] On search, search results page  (https://developers.google.com/youtube/v3/docs/search)
  - [ ] Sort results by date, rating, relevance
- [ ] On selection, Video page (https://developers.google.com/youtube/v3/docs/videos/list?apix_params=%7B%22part%22%3A%5B%22snippet%2CcontentDetails%2Cstatistics%22%5D%2C%22id%22%3A%5B%22Ks-_Mh1QhMc%22%5D%7D)
  - [ ] Title links to video on YouTube
  - [ ] Thumbnail
  - [ ] Description
  - [ ] Display total number of comments on each video
- [ ] Use developer app credentials so sign-in is not required?
- [ ] Dev/prod setups

Note: I started with ideas from https://codepen.io/jorgebucaran/pen/ZeByKv, https://github.com/loteoo/hyperapp-starter, https://codepen.io/jorgebucaran/pen/ZeByKv.

### Extension Ideas

- compression/separation/CI/CD
- Testing
- Video player instead of redirect to YouTube for playback
- Login
  - Use YouTube API library (`<script src="https://apis.google.com/js/api.js"></script>`)
  - Interact with video (Like, Comment)
  - Playlist management


## Components

- Search form
- Video list
  - Video list item
- Video details


# Setup

1. Update `GOOGLE_API_KEY` in `config.js`.
1. Open `app.html` in a browser.


# Original Prompt

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
