#ToS Fiend  

  A collection of popular websites' terms of service documents which are checked regularly against their current values in order to document change and provide a sanitary way to show differences.  
  
###What is this for?

  This is primarily to hold popular online communities accountable for changes they make with or without notification to their userbase and provide an objective view (git diff) of the changes made, which among diff-reading entities provides innate clarity to the changes.
  
### How does it work?

  A scraper (TODO: Make codebase ready for human consumption.) loops over the configuration files ($name.json) and visits the urls provided as sources, checking for changes and committing them where applicable. All of these pieces are automated and run in intervals. Below you will find a sample configuration file.

```json

{
  "name": "example.com",
  "sources": {
    "tos": {
      "url": "http://www.example.com/terms_of_service",
      "element": "div#content"
    }
  }
}

```

  As you can see, the formatting is fairly self-explanatory. The keys for the objects in the sources object are used for filenames and the element provided is used for grabbing only a portion of the page for use in cases where a dynamic or unique hash or code is generated on page load (think CSRF token) but not included in the article.

### How can I add sites to it?

  You can submit a pull request using a branch named after the site with a directory in the root named after the site, containing a json configuration file named after the site with a file extension of .json. It is also necessary to note that you must confirm that the URL or URL and element you provide will result in a non-dynamic output on page load. 
