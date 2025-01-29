[https://apify.com/epctex/youtube-video-downloader](https://apify.com/epctex/youtube-video-downloader?fpr=yhdrb)

# Actor - Youtube Video Downloader

## Youtube Video Downloader

Since Youtube doesn't provide a good and free API to download the videos, this actor should help you to download videos from Youtube.com

The Youtube Video Downloader supports the following features:

-   Download Video - If you want to get videos on a certain URL, just type the URL.

## Bugs, fixes, updates, and changelog

This scraper is under active development. If you have any feature requests you can create an issue from [here](https://github.com/epctex/youtube-video-downloader/issues).


## Input Parameters

The input of this scraper should be JSON containing the list of pages on Youtube that should be visited. Required fields are:

- `startUrls`: (Optional) (Array) List of Youtube video URLs you want to download.

- `quality`: (Optional) (String) The desired video resolution. If the exact quality isn't available, it will default to the nearest lower quality option.

- `proxy`: (Required) (Proxy Object) Proxy configuration.

This solution requires the use of **Proxy servers**, either your own proxy servers or you can use [Apify Proxy](https://www.apify.com/docs/proxy).

### Compute Unit Consumption

The actor is optimized to run blazing fast and scrape as many items as possible. Therefore, it forefronts all the detailed requests. If the actor doesn't block very often it'll scrape 100 videos in 5 minutes with ~0.08-0.10 compute units.

### Youtube Video Downloader Input example

```json
{
  "startUrls":[
    "https://www.youtube.com/watch?v=XqZsoesa55w&ab_channel=PinkfongBabyShark-Kids%27Songs%26Stories",
    "https://www.youtube.com/watch?v=PsNyag6JGv4&ab_channel=RedBull",
    "https://www.youtube.com/watch?v=ctEksNz7tqg&ab_channel=RedBull"
  ],
  "proxy":{
    "useApifyProxy":true
  }
}

```

## During the Run

During the run, the actor will output messages letting you know what is going on. Each message always contains a short label specifying which page from the provided list is currently specified.
When items are loaded from the page, you should see a message about this event with a loaded item count and total item count for each page.

If you provide incorrect input to the actor, it will immediately stop with a failure state and output an explanation of what is wrong.

## Youtube Video Downloader Export

During the run, the actor stores results into a dataset. Each item is a separate item in the dataset.

You can manage the results in any language (Python, PHP, Node JS/NPM). See the FAQ or <a href="https://www.apify.com/docs/api" target="blank">our API reference</a> to learn more about getting results from this Youtube Video Downloader actor.

## Scraped Youtube Video Downloader Properties

The structure of each item in Youtube Video Downloader looks like this:

### Item Detail

```json
{
    "sourceUrl": "https://www.youtube.com/watch?v=ADs8tvU2xDc&ab_channel=RedBull",
    "downloadUrl": "https://api.apify.com/v2/key-value-stores/fpmCnEkWlRujDgf2d/records/ADs8tvU2xDc.mp4"
}
```

## Contact
Please visit us through [epctex.com](https://epctex.com) to see all the products that are available for you. If you are looking for any custom integration or so, please reach out to us through the chat box in [epctex.com](https://epctex.com). In need of support? [business@epctex.com](mailto:business@epctex.com) is at your service.
