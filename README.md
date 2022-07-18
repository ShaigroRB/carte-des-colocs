# What?

This is a dead simple page to help find the latest flatshares posted on [La Carte des Colocs](https://www.lacartedescolocs.fr/).

On the website, you can filter posts by publication date with lowest granularity being "Added today".

I don't think that's enough, so I made this crappy website so it parses and lists the posts sorted by date.

# How to use?
- Go to [La Carte des Colocs on the concerned city](https://www.lacartedescolocs.fr/logements/fr/ile-de-france/paris) (Paris here).
- Press F12 to open the Dev Tools of the browser.
- Go to the "Network" tab.
- Reload the page.
- Look for a request of the form:
  `https://www.lacartedescolocs.fr/listing_search/map_results?token=...`.
- Copy the response of that request. Should be of the form: 
  `{"zoom" : "...", "hashes" : "...", "results" : [...] }`
- Go to https://shaigrorb.github.io/carte-des-colocs/.
- Paste the response in the text area and click "Sort by latest".
- Latest posts are then listed by most recent to least recent.

# Improvements?
Absolutely no guarantee whatsoever.
- Improved filter by categories.
- Improved filter by city.
