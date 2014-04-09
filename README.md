# Heartbleed

List of sites that have fixed there infrastructure against heartbleed.

The idea of this repository came from two tweets from [janl](https://twitter.com/janl/status/453874289528549376) and [rem](https://twitter.com/rem/status/453874447305687040).
We should have some central place where site owner can "notify" everyone that they hardend their infrastructure aginst [The Heartbleed Bug](http://heartbleed.com).

## Contribute
You can contribute your site to this repository via pull requests. Just create a file with the reversed name of your domain.
If github.com wanted contribute their disclosure they would create a file with the name `com.github` with the following contents:

```
{
  "time": 1397057770
}
```

The content is a plain JSON object and can contain the following keys:

- **`time`** – The time after which communications are assumed to be save again
- **`includeSubdomain`** - If also all subdomains have been secured

## Feedback
If you want to provide feedback to this repository: please just create an [new issue](https://github.com/tobiastom/heartbleed/issues/new). 
