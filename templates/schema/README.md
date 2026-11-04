# Schema templates

JSON-LD templates for the Ella Baché Hobart salon pages. Values come from `skills/ella-bache-business`; if a fact changes there, change it here in the same pull request.

| File | Use | Notes |
|---|---|---|
| `beautysalon.jsonld` | The home page and Team & Reviews page of ellabachehobart.com.au | Filled 4 Nov 2026. Hours use the owner's Monday 9 to 4 (conflict with a directory listing is open in ella-bache-business section 10). Still to add once confirmed: `image` (a real photo of the shopfront, hosted on the site), `geo` (latitude/longitude from the Google Business Profile pin), `priceRange`. Holiday hours go in `specialOpeningHoursSpecification` when announced. Only add `AggregateRating` for real reviews shown on the site (e.g. My Local Salon reviews displayed on the page); Google reviews can't be marked up. Head office controls ellabache.com.au: don't propose schema changes there. |

Validate every change with Google's Rich Results Test before it goes live, and get owner approval for any website edit.
