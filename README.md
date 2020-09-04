# Module Project: Component Side Effects- NASA APOD

Consumes the NASA API to fetch the "Astronomy Photo Of The Day" or APOD.  A few components render different pieces of data in the interface. Styled using the styled-components library. Built from scratch. 



-  there is an effect hook to handle the API call side effect.
- the [NASA APOD API docs](https://api.nasa.gov/#apod) docs explain how to make the API call.
- data is fetched from the endpoint using `axios`
- the effect hook has a dependency array (empty, since effect is not synced up to any state/props), to avoid an infinite loop, and to avoid exceeding the API rate limits of the DEMO_KEY

# DEMO KEY rate limits:

> Hourly Limit: 30 requests per IP address per hour
> Daily Limit: 50 requests per IP address per day

_Note: sometimes the photo url is not a photo, but a video. if this is the case, it will not display.
