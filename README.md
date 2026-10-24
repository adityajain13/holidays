# Holidays Calendar

A subscribable `.ics` calendar of Ontario, Canada holidays, observances and cultural dates, covering **1997–2030**. Every event is an all-day event with a single emoji prefix (e.g. `🎉 New Year's Day`, `🪔 Diwali`).

## Subscribe (Google Calendar)

1. Open [`holidays.ics`](holidays.ics) in this repo and click **Raw**. Copy the URL, which looks like:
   `https://raw.githubusercontent.com/adityajain13/holidays/main/holidays.ics`
2. On desktop web: [calendar.google.com](https://calendar.google.com) → **Other calendars (+)** → **From URL**.
3. Paste the raw URL and click **Add calendar**.

Google refreshes subscribed calendars on its own schedule (roughly every 12–24 hours), so new events and edits can take a while to appear. Subscribed calendars sync to the phone app automatically.

> **Don't import the file on top of an existing copy.** Importing adds events again instead of updating them. Subscribe by URL, or delete the old calendar before re-importing.

## What's included

| Group | Events |
|---|---|
| Ontario statutory holidays | New Year's Day, Family Day (from 2008), Good Friday, Victoria Day, Canada Day, Labour Day, Thanksgiving, Christmas Day, Boxing Day |
| Other days off / commonly observed | Easter Monday, Civic Holiday, Remembrance Day, National Day for Truth and Reconciliation (from 2021) |
| Common observances | Valentine's Day, St. Patrick's Day, April Fools' Day, Easter Sunday, Mother's Day, Father's Day, Cinco de Mayo, Halloween, Christmas Eve, New Year's Eve |
| Seasons and clocks | March Equinox, June Solstice, September Equinox, December Solstice, Daylight Saving Time start and end |
| Cultural festivals | Diwali, Choti Diwali, Bhai Dooj, Raksha Bandhan, Ugadi, Makar Sankranti, Chinese New Year |

That is 36 event types and 500 events in total, or about 34–36 events per year (the count rises when Family Day and the Truth and Reconciliation Day begin).

## How the dates were produced

- **Fixed-date and weekday-rule holidays** (e.g. 3rd Monday of February) are written as recurring events, so they keep working past 2030.
- **Daylight Saving Time** uses the old rule (1st Sunday of April to last Sunday of October) through 2006 and the current rule (2nd Sunday of March to 1st Sunday of November) from 2007.
- **Easter, Good Friday and Easter Monday** are calculated for each year with the standard Easter algorithm.
- **Equinoxes and solstices** are calculated astronomically and converted to Toronto time, so the calendar date can differ by a day from UTC listings.
- **Diwali, Raksha Bandhan, Ugadi** and **Makar Sankranti** follow lunar or solar-sidereal calendars, so each year has its own dated event. Diwali and Raksha Bandhan come from published date tables.
- **Chinese New Year** is calculated from the lunar calendar.

### Known caveats

- **Choti Diwali** is set to the day before Diwali, and **Bhai Dooj** to two days after, which matches every year I checked. The one exception is 2028, where Choti Diwali falls on the same day as Diwali. Choti Diwali events outside 2028 are computed, not individually verified.
- **Ugadi** can fall on a different day depending on region and panchang. Dates for 2007, 2008, 2017 and 1998 were checked against published calendars; the rest are calculated.
- **Chinese New Year, Ugadi and Makar Sankranti** were calculated and spot-checked, not compared against a full published table.
- The lunar and cultural events are **not recurring**, so they stop after 2030 and need new dates added for later years.

## Updating

Replace `holidays.ics` in this repo with the new version (same path and filename). The raw URL does not change, and subscribers pick up the update on the next refresh.
