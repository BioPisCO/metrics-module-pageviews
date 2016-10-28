# Metrics Pageviews
This metric obtain the articles pageviews of Wikimedia. It can get pageview trends on specific articles or projects.

## Specification

1. **Resource**: Analytics/Pageview API
2. **Source**:  Wikimedia Foundation
3. **Metric parameters**:
  1. **Query**: keyword or comma-separated articles or projects
4. **Scope**: includes all articles projects from Wikimedia and its sister projects
5. **Library description**: 
  1. **pageviewscount.js**: return the number of views for the last day visited:
  2. **pageviews**.count(keyword, callback): 
    - **keyword**:list of article name(s)..
    - **callback**: function (pageviews, message).
  3. **pageviews.js**:  a lightweight JavaScript client library for the Wikimedia Pageviews API for Wikipedia and various of its sister projects for Node.js and the browser.
 
## Example:
1. **Input**: Uniprot
2. **Query**:   http://wikimedia.org/api/rest_v1/metrics/pageviews/per-article/en.wikipedia/all-access/all-agents/Uniprot/daily/2015100100/2015100100
3. **Output**: 12 views.

> Information about Wikimedia Pageviews API:
    https://wikitech.wikimedia.org/wiki/Analytics/PageviewAPI                   
    pageviews.js based on: https://www.npmjs.com/package/pageviews


## Git

```git clone https://github.com/BioPisCO/metrics-module-pageviews.git```

## Requirements

  1. Nodejs
  2. npm

## Install library dependencies

  ```nmp install```

## Command line execution

```node example/example/example-pageviews.js Uniprot```
