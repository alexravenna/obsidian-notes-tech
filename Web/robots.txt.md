---
created: 2024-04-09T07:03:07Z
updated: 2024-12-10T08:34:54Z
tags:
  - file
  - SEO
documentation:
  - https://developers.google.com/search/docs/crawling-indexing/robots/intro
specification: https://www.rfc-editor.org/info/rfc9309
resources:
  - https://support.google.com/webmasters/answer/7489871
---
# Description
- A standard file for managing [[Web crawler|web crawler]] traffic, i.e. preventing/allowing crawling
- Implements the Robots Exclusion Protocol
	- Was originally a de facto standard from 1994, then published as an [[IETF]] [[RFC]] in 2019 by [[Google/Google|Google]]
- Stored in the web site's home/root directory
- Relies on voluntary compliance, i.e. a crawler can't be forced to follow its instructions
- #caveat Is *not* used exclusively for hiding a web page from search engine indexing
	- The page can still be referenced by other pages and be indexed thereby, just without the crawler visiting them
		- The page will then show up in search results but with no description
- *Can* be used to prevent media files from being indexed by Google search (i.e. they won't be crawled)
# Syntax
```robots.txt
User-agent: *
Allow: /

Sitemap: /sitemap
```
`User-agent`: which crawler/bot should be managed by the succeeding rules
`Allow/Disallow`: a relative path to a file that where crawling should be allowed or disallowed. Multiple entries are possible, as is the use of some special characters: (#, *, $).  `/` refers to all content on the site
`Sitemap`(non-standard): the location of the website's [[Sitemap|sitemap]]

Multiple `User-agent` blocks can be used, defining different rules for different bots