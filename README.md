# Commute Launchpad

[Open the dashboard](https://kevalpatel370-commits.github.io/commute-launchpad/)

A responsive, single-file morning commute dashboard from Deptford to Monroe, NJ. Published using GitHub Pages from the root of the main branch.

## Camera setup

All 11 camera slots initially display labeled placeholders, not live traffic. Edit each image's `data-src` in `index.html` to use a verified HTTPS static camera image URL. Update its heading and alt text to match the verified feed. A camera web page is not a direct image URL.

The dashboard requests new images every 30 seconds, on manual refresh, and when returning to the page. Browsers can suspend background timers. Image download times do not verify when the camera captured an image; source servers may also cache snapshots.

## Route links

Three Google Maps buttons open the primary Exit 5 route, fallback Exit 4 route, and route starting at Woodcrest Station. Review the calculated path: waypoints do not force every road or guarantee current ramp access. Route 55 joins Route 42, and the Evesham bypass requires connecting local roads. The requested MM 71.0 slot is an approach view; NJTA identifies its Exit 8A camera at MM 73.7.

## Updating the website

Edit and commit `index.html` on `main`. GitHub Pages automatically republishes it. No build tools, paid hosting, or API keys are required. This repository and website are public, including the commute addresses in the dashboard.
