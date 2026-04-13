# Venue

The Sorrento Meeting is held at the **Grand Hotel Vesuvio**, Sorrento, Italy. This venue is pre-filled in `_config.yml` — if the meeting ever moves, update the `conference.venue`, `conference.venue_url`, and `conference.location` fields.

## Confirming the Dates

The meeting has historically been held in late March / early April. The precise dates need to be agreed with the hotel. Check availability early — the hotel is popular and blocks of rooms need to be reserved well in advance.

Contact: concierge@vesuviosorrento.com

Once you have confirmed dates, update the `_config.yml` file:

```yaml
conference:
  dates:
  - YYYY-MM-DD
  - YYYY-MM-DD
  - YYYY-MM-DD
```

Include each day the meeting will run. They are used by the theme when generating the programme.

Note the use of [ISO standard date format](https://en.wikipedia.org/wiki/ISO_8601) — as an international meeting we use international dates.

## Room

The main conference room has historically been the **Turchese** room. Update `conference.room` in `_config.yml` if this changes. The room name is also referenced in each `_posts/` programme file.

## Getting the Timing Right

Getting the precise dates confirmed is a critical first step, because the rest of the meeting organisation works backwards from there.

Also think about whether you want to pre- or post-conference days (e.g. a welcome reception evening). The template includes a `XXXX-MM-DD-day-0.md` post as a placeholder for this.

[Go back to main doc README.md](./README.md)
