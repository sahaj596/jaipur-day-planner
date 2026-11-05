# Jaipur in a Day

A one-day itinerary planner for visitors to Jaipur, Rajasthan.

## Problem
Visitors lose hours to poor routing, places that are closed on arrival, crowds at the wrong time of day and surprise costs. Most guides list attractions but do not turn them into a workable day.

## What it does
Enter your date, starting area, start and finish times, budget per person, group size, interests and pace. The planner builds a timed route that:

- respects each place's opening hours and typical closures (for example Sunday market closures)
- prefers the best time of day for a place (early for Amer Fort, sunset for Nahargarh and Jal Mahal)
- estimates ride time, distance and fare between stops, split across your group
- applies Indian or international entry fees and stays within your budget
- inserts a lunch stop around midday
- surfaces lesser-known places such as Panna Meena ka Kund and Galta Ji
- lists what was left out and why, with a copy-as-text option

## Run it
It is a single static file with no build step. Open `jaipur-day-planner.html` in a browser.

## How it works
Places are scored by popularity, interest match and time-of-day fit, minus travel and waiting time. The route is built greedily: from the current location and time, it picks the best feasible next stop until time or budget runs out.

## Data notes
Fees, hours, fares and some coordinates are approximate planning figures entered by hand. Confirm on arrival.

## Ideas for next steps
- verified opening hours and fees from official sources
- live traffic and weather
- community-contributed hidden gems
- more cities using the same engine
