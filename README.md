# Commute Launchpad

[Open the dashboard](https://kevalpatel370-commits.github.io/commute-launchpad/)

A responsive, single-file morning commute dashboard from Deptford to Monroe, NJ.

## Live feeds

The Turnpike cards use official NJTA HLS camera streams for verified locations including Interchange 3, Interchange 4, north of Interchange 5, north of Interchange 8, and Interchange 8A. The dashboard lazily starts streams when they are near the viewport and refreshes stream URLs every 30 seconds. Local RT 42, Route 55, Evesham, and I-295 camera cards link to the official 511NJ viewer because its player requires the site’s authenticated session and does not expose embeddable public image URLs.

## Route prioritization

The dashboard includes a normal OpenStreetMap view, Google Maps links for each branch, transparent manual comparison of current Maps times, and an optional TomTom traffic-routing connection. Enter a TomTom key in the page only when you want automatic traffic comparison; it is held in memory for that session and sent with the commute locations only after you click Connect. The advisor ranks traffic-adjusted route estimates and explains the recommendation. Without a provider key, it uses your selected merge/highway conditions and any Maps times you enter; it never pretends that an unavailable feed is clear.

## Updating

Edit and commit `index.html` on `main`. GitHub Pages automatically republishes it. No provider key is stored in this repository. Review current camera directions, incidents, closures, tolls, and the calculated route before leaving.
