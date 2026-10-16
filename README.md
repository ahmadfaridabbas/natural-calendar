# Natural Calendar

A TinyCast / Raycast extension that creates Apple Calendar events from natural language, e.g. _"Lunch with Sam tomorrow at 1pm"_.

## Commands

- **Create Calendar Event** — type an event in plain English via a UI and add it to Apple Calendar.
- **Quick Add Calendar Event** — add an event from a single text argument, no UI.

## Preferences

- **Default Calendar** — name of the calendar new events are added to (must match a calendar in Calendar.app exactly). Default: `Calendar`.
- **Default Duration (minutes)** — event length when no end time is given. Default: `60`.
- **Default Start Time (HH:MM, 24h)** — start time used when the text has a date but no time. Default: `09:00`.

## How it works

- [`chrono-node`](https://github.com/wanasit/chrono) parses the natural-language date/time.
- [`run-applescript`](https://github.com/sindresorhus/run-applescript) adds the event to Apple Calendar.

## Development

```bash
npm install
npm run dev
```

## Author

faridabbas

## License

MIT
