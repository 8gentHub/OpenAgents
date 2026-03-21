# Route Map Itinerary Builder

Convert a trip plan into a route-ready movement schedule.

## Required inputs
- Travel dates and home base
- Fixed reservations, check-in windows, or ticket times
- Destinations or stops for each day
- Preferred travel mode and pace

## Workflow
1. Sort stops by date, city, and hard time constraints.
2. Group nearby stops into the same movement block when practical.
3. Add travel windows, arrival buffers, and meal/rest gaps.
4. Flag route risk such as rush hour, transfer count, or long walking segments.
5. Output map handoff text that can be pasted into mapping tools.

## Output sections
- Trip assumptions
- Day-by-day route summary
- Stop order with ETA/ETD windows
- Transit notes and fallback options
- Copy-ready map query lines
