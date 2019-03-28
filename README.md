# Amazon Reviews Crawler Go

## Summary

Simple tool to crawl Amazon Reviews metadata from product ID(s).
If running via terminal, simply pass the list of product ID(s) as argument, and pass the optioonal `-out=output.json` flag to export resulted json to `output.json` file.

If you want to crawl from different Amazon regional website, you can pass either `uk` or `us` optional region flag, if region mapping isn't found, region flag input will be used as website domain suffix.


First iteration is scripted in Python and is located at [here](https://github.com/anzellai/amazon_reviews_crawler)


## Setup

`go get`


## Example

Crawling product ID "ABCDE", and run:

`go run cmd/crawler/crawler.go -region=uk -out=output.json ABCDE`


Or, run existing pre-built binary from `/bin` directory:

`./bin/amazon-reviews-crawler-go-darwin -region=uk -out=output.json ABCDE`
