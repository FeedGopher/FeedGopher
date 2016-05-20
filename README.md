# FeedGopher
An offline-capable Atom reader Chrome Extension

RSS - rich site summary  |  really simple syndication

XML format

application/rss+xml

Chrome extension
  flexbox view
  Use web worker / chrome worker to catch requests, check for local cache or no network, and respond.
golang server distributing updates
postgres document storage
Chrome notification

Go server, parses feed, aggregates content,
extension saves docs to local storage

FeedGopher primarily serves as an opportunity to play with a bunch of tools and technologies:

- The Go language
-	SQL through Postgres
	- Postgres as a document store
- RxJS
- HTML/CSS
- Designing application interfaces
- Browser/Chrome utilities
	- persistent storage (local redis?)
	- chrome extension
	- chrome notifications (web worker, )

It is comprised of three primary components:
- Golang server to handle ATOM feeds and users
- PostgreSQL database storing feed items as documents
- Chrome extension using web workers, persistent/offline storage, and request interception/cacheing.