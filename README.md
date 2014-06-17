# Everysport API
The Everysport API gives you access to tables, results and events for 90,000 teams and 1,500,000 matches from [everysport.com](http://www.everysport.com).  

Game events (e.g. goals) reported live on everysport.com is available via the API. For example, if your team uses Everysport for live reports, you can build applications with the data from the API. 

Access to game reports from other leagues (e.g. International) can also be provided by Everysport. Contact <sales@everysport.com> for details. 

The API is REST API with JSON as the return format for all endpoints. 

***

## Getting Started
1. Explore the API documentation [here](/endpoints) to see if this is what you are looking for.
2. Read the Everysport [API Terms of Use](basics/terms_of_use.md).
3. Get your API key, see below.   
4. Build a Great Sports App! 

## Basic
* [Formats and Terms](basics/formats_and_terms.md)
* [Design Principles](basics/design_principles.md)
* [API Terms of Use](basics/terms_of_use.md)

## Endpoints
All endpoints are documented in [endpoints](endpoints/)

## Apply for an API key
In order to use the API you need an API key, here are a few things to bear in mind before you get started:

* Attribution: You must display "Provided by Everysport.com" wherever Everysport data is used.
* Linking: You must link to Everysport teams and events wherever you display such data.
* Exclusivity: You must not combine Everysport data with similar data from other sources. 
* You may only make calls to the Everysport API at a reasonable rate. 
* You may not store Everysport data for any other purpose than caching for a short period of time. 
* You must tell us if you start using the data for Commercial use, we reserve rights to revoke access if this is not complied with. Commercial use is defined as using the Everysport Data for the purposes of monetary reward by means of the sale, resale, loan, transfer, hire or any other form of exploitation of the Everysport Data.
* We have the right to revoke access if your use of the data competes with products or services offered by Everysport. For example, Everysport.com is today one of the largest providers of sport data to media in Sweden, and a large online sport community.

The full Terms of Use are [here](/basics/terms_of_use.md). 

To get an API key, please send us an [email](mailto:support@everysport.com) to <support@everysport.com> with the following information: 
* Your email address
* The domain where the Everysport data will be published (the API-key will be associated with the domain)
* Brief description of the app you are building. 
* Statement saying you agree to comply with the Everysport API [terms of use](/basics/terms_of_use.md)

We contact you as soon as we can. 

## Rate Limits
To protect Everysport the API has a rate limit. By default it's set to 240 calls/h and max 1000/month, for one API user. The limit may change in the future.

## Commercial Use
Please contact us at [support@everysport.com](mailto:support@everysport.com) to obtain a license for commercial use. 

## Discussions Google Groups
Feel free to ask questions in our [Everysport Developer Group](https://groups.google.com/d/forum/everysport-developer).
We will also post updates about new releases there.

## SDKs
The official [Java SDK](https://github.com/menmo/everysport-java-sdk) and [PHP SDK](https://github.com/menmo/everysport-php-sdk) is maintained by [Menmo](http://menmo.se). 

Here are some additional SDKs you can find on GitHub:

* [Python](https://github.com/peterstark72/everysport) by [Peter Stark](https://github.com/peterstark72)
* [Node](https://github.com/carlgrundberg/everysport-node-sdk) by [Carl Grundberg](https://github.com/carlgrundberg)

## Other Resources
Applications that use the API are sometimes published on the [Menmo blog](http://www.menmo.se/blogg/) (in swedish).






  








