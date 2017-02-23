# tweet-search
Final project for independent study of Apache Solr

The Solr core defined here provides two request handlers
  1. /select
    1. This endpoint provides the search capability for the core and has a couple of additional features.
      1. Hit Highlighting: By default, hit highlighting is enabled, showing you the most relevant parts of the tweets you are searching for.
      2. Faceting: Search results also come with facets based on the favorite count of the tweets. The facets are from 0 to 10,000 in increments of 250.
      3. Spellchecking: The core will return similar search terms that provide better results when you query it.
  2. /suggest
    1. This endpoint will provide auto-complete suggestions based on the query string you send it. The suggestions will be generated from the core's contents and can make the search experience more pleasent for the end user.
