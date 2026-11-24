---
name: show-the-work
description: Finish every substantial task (a trip plan, research, a code change, a merge, a deploy, a fix) with a presentable page with real pictures instead of a "done" message. Use whenever work produced something the owner should see or decide on, especially in sessions started from the phone via Remote Control.
---

# Show the work

"Done" is not a report. The owner wants a page they can open on the phone and understand in a minute, with pictures.

## Every result page has

1. **One-line outcome** at the top: what happened, and the one thing needed from the owner (or "nothing").
2. **Pictures.** No page ships without them.
   - Code/UI change: screenshots **before and after**, phone width (390) first, then desktop (1440). Take them yourself (Playwright or the box's Chrome), look at them before using them.
   - Trip / place / product: real photos of the actual place or item. Sources in order: the venue's or official site's own images, Wikimedia Commons (credit the author and licence under the photo), screenshots you took of the live page (prices, listings, maps). Never AI-generated images presented as real places.
   - Data: a chart, not a table, when there are more than ~5 numbers.
   - **Every media item has a Download button**: each video, picture and file on a page gets a clear Download button that saves the full-quality file, not the light web preview. Use a plain `<a href=".." download>` next to each item, 44 px tall, on its own line on a phone.
3. **Why** for each change or choice: what it improves, in plain words.
4. **Evidence**: links to the sources, prices with the date and time you checked them, test/build output quoted from the log, the PR or preview link.
5. **Open questions / decisions** as a short list at the end.

## How

- Publish with the Artifact tool (load `artifact-design` first). Upload photos and screenshots to the artifact's asset store and reference them by the returned URL; don't hotlink.
- Trip pages: day-by-day itinerary with a photo per stop, the reason it is on the list, cost, how to get there, and a budget total. Flights and stays show the live price screenshot.
- Code pages: summary, before/after pairs, what changed and why, review findings (from a different model) and how each was handled, test/build results, how to try it.
- Send the link back in the reply as the last line. Keep the reply itself to 3–5 lines; the page carries the detail.

## Don't

- Don't write "it should work". If it wasn't checked, the page says "not verified" next to it.
- Don't put credentials, tokens or private personal details on the page.
