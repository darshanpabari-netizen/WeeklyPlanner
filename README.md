# Weekly Schedule Planner

A self-contained browser-based planner for designing a repeating weekly routine.

![Weekly Planner Screenshot](./screenshot-placeholder.png)

## Features

- Weekly grid view with Monday–Sunday columns and a configurable time range in 30-minute increments (default 6:00 AM to 11:00 PM)
- Sticky day headers and sticky time column for easier scrolling
- Add, edit, and delete events with name, day, start/end time, category, and optional notes
- Event blocks color-coded by category and rendered with overlap-aware side-by-side layout
- Built-in category management: add, rename, recolor, and delete categories
- Safe category deletion flow with event reassignment when the category is in use
- Weekly summary panel with total hours, hours by category, and percentage bars (pure CSS)
- Settings for visible time range, theme toggle (light/dark), and clearing all events
- Automatic localStorage persistence for events, categories, and settings
- JSON export/import for backup and restore
- Keyboard-accessible modals (Esc to close, Tab focus loop)
- Narrow-screen guidance and print-friendly layout

## Use cases

This tool is for anyone planning a template week rather than date-specific events: students managing classes and study sessions, professionals mapping work blocks and routines, freelancers balancing client time, and anyone organizing recurring weekly habits.

## How to use

1. Open `index.html` in any modern web browser.
2. Click an empty time slot (or **+ New event**) to add an event.
3. Click an existing event to edit or delete it.
4. Use **Settings** to change time range, theme, and categories.
5. Use **Export JSON** to back up and **Import JSON** to restore/replace data.

No setup, server, build tools, or dependencies are required.

## Data storage

All planner data is stored in your browser via `localStorage`.

- Includes events, categories, and UI settings.
- Data stays on the same browser/profile/device unless exported.
- Use **Export JSON** regularly for backups.

## Customization

Open **Settings** (⚙) to:

- Change visible start/end time range for the weekly view
- Toggle between light and dark themes
- Add a category with custom name and color
- Rename/recolor existing categories
- Delete categories (with reassignment prompt if events use that category)
- Clear all events with confirmation

## Keyboard shortcuts

- **N**: Open add-event modal
- **Esc**: Close open modal
- **Tab / Shift+Tab**: Navigate modal controls

## Browser compatibility

Works in modern versions of:

- Google Chrome
- Mozilla Firefox
- Microsoft Edge
- Safari

## Limitations

- No cloud sync or cross-device synchronization
- No multi-user collaboration
- Template-week planner only (no specific dates or recurring rules engine)
- Import replaces current data (with confirmation)

## Future ideas

- Drag-and-drop moving and resizing of events
- Optional day-grouped list view for small screens
- Multiple planner templates/presets
- Per-event reminders and notifications
- Optional CSV export
