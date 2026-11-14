# TRPL Event Floor Planner

An interactive, to-scale event floor planner for four spaces at the Theodore Roosevelt Presidential Library:

- Main Lobby (W100)
- White House Facade (W166)
- Prefunction Space (Auditorium Lobby E100 + Prefunction E101)
- The People's Library (W185)

Drag tables, chairs, stages, bars and more onto a plan traced from the architectural drawings, check fit and aisle widths, assign seats, and walk through each room in a 3D view (day or night).

## Running it

It is a single self-contained page: open `index.html` in a browser, or serve it with GitHub Pages (Settings → Pages → deploy from the `main` branch).

## What works where

This page was built as a Claude artifact. Some features rely on capabilities that only exist when it is opened on claude.ai:

| Feature | On claude.ai | Standalone (this repo) |
|---|---|---|
| Planning, fit checks, 3D view, seating by hand | Yes | Yes |
| Saved layouts | Shared with your team, live co-editing | Saved in this browser only |
| "Suggest a layout" and the Seating assistant (AI) | Yes | Not available |
| PNG and CSV downloads | Yes | Yes (ordinary browser download) |

When the page is opened outside claude.ai, an **Open the full planner on claude.ai** button appears in the header, and the AI tools and Layouts dialog link there too, so staff can switch to the full version with shared layouts and the AI tools (they need to be signed in to claude.ai).

## Sharing layouts

The **Share** button in the header works on both versions:

- **Share link**: a link that opens a copy of the layout, with its seating and tags. Links always open this website copy; paste one under *Open a shared layout* to bring it into the claude.ai version.
- **Layout file**: one HTML file that opens in any browser as a printable seating report (setup, meal and allergy totals, every table's seating with tags, and an A–Z guest list), and can be loaded back into the planner with *Choose layout file*.

Both are snapshots: they don't update when the layout changes later.

The 3D view loads three.js from cdnjs and jsDelivr, so it needs an internet connection.