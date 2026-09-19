# Universities of Kazakhstan

A one-page directory of the official websites of Kazakhstan's major
universities — 70 institutions grouped by region, plus the international branch
campuses that have opened in the country. Plain HTML, CSS and JavaScript with a
live search box; no build step, no dependencies.

Live: https://ktwyw.github.io/kz-universities/

## What's included

- **National and research universities** in Astana and Almaty (Nazarbayev
  University, ENU, KazNU, Satbayev, KBTU, KIMEP, the national medical,
  pedagogical and agrarian universities, and others)
- **Regional universities** in every part of the country: Shymkent and
  Turkistan, Karaganda, East, North, West and South Kazakhstan
- **Specialist institutions**: medical universities, arts academies, the
  conservatory, sports, architecture, transport
- **International branch campuses**: Cardiff, Coventry and De Montfort (UK)
  and Lomonosov Moscow State University

The search box filters by name, city or field as you type, so "medicine"
lists the medical universities and "Aktobe" lists that city.

## How to add or correct a university

All data lives in one array near the top of the script in `index.html`:

```js
["Name as commonly written in English", "https://official-site", "Region group", "city; short tag"],
```

Add a line in the right region block, then open a pull request. Please link
the university's own site, not a ranking or directory page.

## Notes

- Links were checked in September 2026. University domains change (for
  example after a rename), so if one fails, search the name.
- "National" in a tag marks universities that hold national status.
- The list aims for the influential and widely known institutions, not every
  licensed provider — Kazakhstan has over a hundred.

## Ideas for next steps

- Add Kazakh and Russian names to each entry and a language switch
- Add each university's city on a map (Leaflet + a small GeoJSON file)
- Pull QS/THE ranking positions into the tags
