# A worked example with dc.js
Rebuilding the dc.js Nasdaq example step-by-step

The Nasdaq dashboard can be seen here:
* [https://dc-js.github.io/dc.js/](https://dc-js.github.io/dc.js/)

The annotated code is here:
* [https://dc-js.github.io/dc.js/docs/stock.html](https://dc-js.github.io/dc.js/docs/stock.html)

In this repo, I'm going to add things step by step so that I understand what's going on in greater detail. Most code will go in `dashboard.html`.

To run the example and see all the graphs, set up a local server with either:
* `python -m SimpleHTTPServer`
* `python3 -m http.server`
* Any server of your choice

Then in your browser go to `localhost:8000/dashboard.html` (replace the port or URL as required by your server set-up).


## Steps

1. create an HTML skeleton and pull in the required libraries from a CDN.
2. download data, load the CSV with d3, coerce strings to the right formats, then load it into CrossFilter
3. Create a simple datatable that displays all the data in rows
4. Add in bootstrap and make the table look nice
