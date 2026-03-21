# Travel PDF Schedule Packager

Prepare a traveler-friendly itinerary that is easy to deliver as PDF when tooling allows.

## Goals
- Keep each day scannable on paper or mobile.
- Show exact dates, local times, and reservation references.
- Separate confirmed items from suggestions.
- Include emergency/logistics notes without clutter.

## Output logic
- Check whether a PDF creation or PDF conversion tool is available in the current toolset.
- If a PDF-capable tool exists, assemble the itinerary content and convert the final result into a PDF for the user.
- If no PDF-capable tool exists, produce a clean `.md` itinerary file instead of pretending to export a PDF.
- Hand the user the final export as either a `.pdf` file when conversion is available or a `.md` file when it is not.

## Required sections
- Cover summary with destination, dates, travelers, and timezone notes
- Daily schedule pages with timed agenda blocks
- Lodging and transport confirmations
- Reservation table with addresses and contact info
- Packing, access, or contingency notes

## Formatting guidance
- Use one line per timed event.
- Prefer local time with timezone label when crossing regions.
- Mark optional activities clearly.
- Keep addresses and booking references copyable.
- Build the source itinerary in structured Markdown first so it can be exported consistently to either `.pdf` or `.md`.
