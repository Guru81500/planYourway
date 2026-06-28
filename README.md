# Plan My Way

Plan My Way is a simple travel itinerary planner built with HTML, CSS, and vanilla JavaScript. It helps users create day-by-day travel plans, add destinations and activities, save plans locally, and preview, share, or print their itinerary.

## Features

- Create multiple itinerary days
- Add an optional date for each day
- Add day-level notes
- Add destinations with name, time, and notes
- Add activities with name, time, and notes
- View live totals for days, destinations, activities, and total itinerary items
- Save and reload itinerary data using browser `localStorage`
- Preview the full itinerary in a modal
- Share the itinerary using the browser share API when available
- Copy the itinerary text to the clipboard as a fallback
- Print the itinerary from the preview view
- Submit a simulated contact form with success feedback

## Pages

- `index.html` - Home page with a short introduction and feature list
- `itinerary.html` - Main itinerary planner
- `contact.html` - Contact form and support information
- `style.css` - Shared styling for all pages

## How To Use

1. Open `index.html` in a browser.
2. Go to the `Itinerary` page.
3. Select `Add Day` to create a travel day.
4. Optionally add a date and day notes.
5. Add destinations or activities for that day.
6. Use `View Itinerary` to review the full plan.
7. Use `Share Itinerary` or `Print` when ready.

No build tools or package installation are required.

## Data Storage

The itinerary is saved in the browser using `localStorage`. This means:

- Saved itinerary data stays available after refreshing the page.
- Data is stored only in the current browser on the current device.
- Clearing browser storage or selecting `Clear All` removes the saved itinerary.

## Accessibility Notes

The app includes several accessibility-focused improvements:

- Semantic page structure with header, navigation, main content, and footer
- Accessible labels for itinerary form fields
- Screen-reader labels for icon-only remove buttons
- Live status messaging for save and contact form feedback
- Keyboard-visible focus outlines
- Improved color contrast for headings, buttons, and important text
- Dialog semantics for the itinerary preview modal

## Testing Checklist

Recommended manual checks:

- Add a day and verify the empty state disappears
- Add a date and verify it appears once in `View Itinerary`
- Add a destination and activity and verify summary totals update
- Refresh the page and verify saved itinerary data reloads
- Share the itinerary and verify text output includes day dates
- Print the itinerary preview
- Clear all data and verify the empty state returns
- Submit the contact form and verify the success message appears
- Navigate the main controls using the keyboard

## Project Status

This is a static front-end project. Future improvements could include destination suggestions, drag-and-drop reordering, exporting to PDF, or syncing itineraries across devices.