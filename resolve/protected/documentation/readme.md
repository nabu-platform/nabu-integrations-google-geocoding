# Components

The components that can be filtered include:

- postal_code matches postal_code and postal_code_prefix.
- country matches a country name or a two letter ISO 3166-1 country code. The API follows the ISO standard for defining countries, and the filtering works best when using the corresponding ISO code of the country. 
    
The following components may be used to influence results, but will not be enforced:

- route matches the long or short name of a route.
- locality matches against locality and sublocality types.
- administrative_area matches all the administrative_area levels.

E.g. https://maps.googleapis.com/maps/api/geocode/json?address=high+st+hasting&components=country:GB&key=YOUR_API_KEY

# Regions

In a Geocoding request, you can instruct the Geocoding service to return results biased to a particular region by using the region parameter. This parameter takes a ccTLD (country code top-level domain) argument specifying the region bias. Most ccTLD codes are identical to ISO 3166-1 codes, with some notable exceptions. For example, the United Kingdom's ccTLD is "uk" (.co.uk) while its ISO 3166-1 code is "gb" (technically for the entity of "The United Kingdom of Great Britain and Northern Ireland").

E.g. https://maps.googleapis.com/maps/api/geocode/json?address=Toledo&region=es&key=YOUR_API_KEY