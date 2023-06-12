
## What does Angi (Angie's List) Scraper do?
Our free Angi (formerly Angie’s List) Scraper let you supercharge your extraction of Angie's List data. By using this unofficial Angie's List API you'll get:

- **Company contact details:** name, email, phone number, address (state, city, street, zip code), working hours, website.

- **General information:** description, logo, media, offered services, services not offered,  payment options, categories, business highlights, awards & badges, amenities, licensing, deals, founded date, registration date (on Angi), and rating details.

- **Company reviews that include:** client name, rating, review text, review details (description of work, work categories, work cost, media), and posting time.

## Need more Angie’s data?
Use [Angi (Angie's List) Scraper](https://apify.com/babak/angi-angie-s-list-scraper) to enjoy the full potential of scraping Angi. Scrape company contact details, general information, and company reviews without limitations in result’s amount.

## How to scrape Angi (Angie's List)
It's easy to scrape Angi with Free Angi (Angie's List) Scraper. Just follow these few steps, and you'll get your data in a few minutes.

1.  Click on Try for free.
2.  Enter the search terms or location you want to scrape.
3.  Click on Run.
4.  When Angi (Angie's List) Scraper has finished, preview or download your data from the Dataset tab.

## Input

| Field Label        | Object Key         | Type     | Description                                                                                                                                                                                                  | Default                    |
|--------------------|--------------------|----------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|
| Location           | location           | string   | Location name as you would search: City name, ZIP code, state.                                                                                                                                               | "Portland"                 |
| Category           | category           | string   | Select a category from                                                                                                                                                                                       | none                       |
| Include reviews    | includeReviews     | boolean  | Is list of reviews should be included to result                                                                                                                                                              | true                       |
| Company page URLs  | directLinks        | string[] | A list of company page URLs can be added as a file,  remote file or just a list of URLs                                                                                                                      | []                         |
| Category page URLs | categoryLinks      | string[] | A list of category URLs, can be added as a file,  remote file or just a list of URLs                                                                                                                         | []                         |
| Zip Codes          | zipcodes           | string[] | A list of US Zip Codes can be added as a file,  remote file or just a list of zip codes                                                                                                                      | []                         |
| Max concurrency    | maxConcurrency     | integer  | Defines how many pages can be processed by the scraper in parallel.  The scraper automatically increases and decreases concurrency based on available system resources. Use this option to set a hard limit. | 100                        |
| proxyConfiguration | proxyConfiguration | object   | Proxy settings of the run. If you have access to Apify proxy, you can set { "useApifyProxy": false" } to disable proxy usage                                                                                   | { "useApifyProxy": true } |

 **To start scrapping, please use at least one search field*

## Results
You'll get a dataset containing the output of this actor. The length of the dataset will depend on the amount of results you've set/got. You can download those results as an  _Excel, HTML, XML, JSON,_  and  _CSV_  document or you can just use [Apify API](https://docs.apify.com/api) to get the data.

Here's an example of scraped Angi data you'll get if you decide to scrape all data from company page "[Design Fab](https://www.angi.com/companylist/us/or/portland/design-fab-reviews-6192675.htm)" .

```json
{
    "city": "portland",
    "state": "or",
    "companyName": "Design Fab",
    "companyDescription": "We specialize in modern and creative architectural interiors for your home or business! Unique design, quality craftsmanship, and a great client experience is what we strive to achieve with every project we do. Custom made entertainment centers, feature walls, bathrooms, kitchens, shelving units, custom furnishings, anything you need or can dream is within our capability, Were great at working together with our clients on a design solution that fits both their needs as well as there personality and style. Contact us to set up a free initial in home design consultation and see for yourself why everybody loves us and our product!Custom woodworking, cabinets, built-ins, custom furniture, renovations, structural & general remodeling, play houses, loft spaces",
    "companyLogo": "https://media-content.angi.com/f1cd3e9c-d160-482b-a388-d77a2a5d9bc2.JPG?imwidth=90",
    "url": "https://www.angi.com/companylist/us/or/portland/design-fab-reviews-6192675.htm#deals",
    "categories": [{
        "name": "Finished Carpentry and Woodworking",
        "link": "https://www.angi.com/companylist/portland/woodworking.htm"
    }],
    "servicesOffered": [
        "Custom woodworking",
        "cabinets",
        "built-ins",
        "custom furniture",
        "renovations",
        "structural & general remodeling",
        "play houses",
        "loft spaces"
    ],
    "servicesNotOffered": [
        "floor"
    ],
    "paymentOptions": [
        "Check",
        "Visa",
        "MasterCard",
        "PayPal"
    ],
    "contactInfo": {
        "address": {
            "googleMapLink": "https://maps.googleapis.com/maps/api/staticmap?center=308%20NE%20Mason%20St%2CPortland%2COR%2C97212&key=AIzaSyAGGS0Q7dARjRia9UK9rL_5PaKDiyMTxU4&mapType=roadmap&markers=color%3Ared%7Clabel%3A%E2%80%A2%7C308%20NE%20Mason%20St%2CPortland%2COR%2C97212&size=336x175&zoom=13",
            "fullAddress": "308 NE Mason St,Portland,OR,97212",
            "detailAddress": {
                "number": "308",
                "prefix": "NE",
                "street": "Mason",
                "type": "St",
                "city": "Portland",
                "state": "OR",
                "zip": "97212"
            }
        },
        "contactsInfo": {
            "phone": "+15037202745",
            "website": "http://www.designfabpdx.com"
        },
        "additionalContactInfo": {
            "name": null,
            "description": null,
            "primaryPhoneNumber": "5037648604",
            "email": "designfabpdx@gmail.com",
            "website": "http://www.designfabpdx.com",
            "inBusinessSince": 2009,
            "onAngiesListSince": "2011-02-09",
            "twilioNumber": "+15037202745"
        }
    },
    "media": [
        "https://media-content.angi.com/tampa/36953891/service_provider/10996901/photo/0751319c7d934efebf10cc82c0307bbb-1465234817.872324.png",
        "https://media-content.angi.com/e4f6e24e-92dd-46c6-8da2-1976cab22411.jpg",
    ],
    "workingHours": [{
            "hoursType": "OpenHours",
            "startTime": "09:00",
            "endTime": "17:00",
            "day": "Monday"
        },
        {
            "hoursType": "OpenHours",
            "startTime": "09:00",
            "endTime": "17:00",
            "day": "Tuesday"
        },
        {
            "hoursType": "OpenHours",
            "startTime": "09:00",
            "endTime": "17:00",
            "day": "Wednesday"
        },
        {
            "hoursType": "OpenHours",
            "startTime": "09:00",
            "endTime": "17:00",
            "day": "Thursday"
        },
        {
            "hoursType": "OpenHours",
            "startTime": "09:00",
            "endTime": "17:00",
            "day": "Friday"
        }
    ],
    "awardsAndBadges": [
        "Angi Certified"
    ],
    "businessHighlights": [{
            "text": "Women Owned & Operated",
            "img": "https://reference-media.angi.com/images/WomenOwned.png"
        },
        {
            "text": "LGBTQ+ Friendly",
            "img": "https://reference-media.angi.com/images/LGBTQFriendly.png"
        },
        {
            "text": "Emergency Services Offered",
            "img": "https://reference-media.angi.com/images/EmergencyServices.png"
        },
        {
            "text": "Eco Friendly",
            "img": "https://reference-media.angi.com/images/EcoFriendly.png"
        }
    ],
    "amenities": [{
            "label": "Free Estimates",
            "val": "Yes"
        },
        {
            "label": "Warranties",
            "val": "Yes"
        },
        {
            "label": "Eco-Friendly Accreditations",
            "val": "Yes"
        }
    ],
    "licensing": [
        "Licensed",
        "Bonded",
        "Insured"
    ],
    "deals": [{
        "link": "https://member.angi.com/app/offer/search/80696?placementType=Web_LeafPage",
        "title": "$100 Credit Toward Cabinet Making"
    }],
    "founded": "2009",
    "withAngiFrom": "since february 2011",
    "reviewsDetail": {
        "rating": "4.8",
        "amountReviews": "93",
        "ratingDetails": [{
                "title": "Price",
                "rating": "4.6"
            },
            {
                "title": "Professionalism",
                "rating": "4.8"
            },
            {
                "title": "Punctuality",
                "rating": "4.8"
            },
            {
                "title": "Quality",
                "rating": "4.8"
            },
            {
                "title": "Responsiveness",
                "rating": "4.8"
            }
        ],
        "ratingDistribution": [{
                "ratingNumber": "5",
                "ratingAmount": "75"
            },
            {
                "ratingNumber": "4",
                "ratingAmount": "7"
            },
            {
                "ratingNumber": "3",
                "ratingAmount": "7"
            },
            {
                "ratingNumber": "2",
                "ratingAmount": "1"
            },
            {
                "ratingNumber": "1",
                "ratingAmount": "3"
            }
        ]
    },
    "reviews": [{
        "userName": "Jared I.",
        "rating": "5.0",
        "date": "09/02/2016",
        "desc": "Terry and team were great to work with. Very collaborative during the design process, with an attitude of \"yes, we can make that work.\" His estimate was roughly 60% of a competing cabinetry-maker. And the communication and install was as promised. Terry even came back to drill additional holes for wires at no cost. All in all, we are extremely satisfied with the final product, and would absolutely hire Terry again.",
        "reviewDetails": [{
                "label": "Description of Work ",
                "text": "Customer cabinetry for a media center and books shelves surrounding our mantle."
            },
            {
                "label": "Category ",
                "text": "custom cabinets, interior designers, custom furniture, woodworking"
            },
            {
                "label": "Cost ",
                "text": "$5,500"
            },
            {
                "label": "Hire Again? ",
                "text": "Yes"
            }
        ]
    }]
}
```
 **Object additionalContactInfo, can be unavailable in the future*

<!-- ## Tips for scraping
- For speeding up the scraping process, we recommend to use this parser in addition with our [Angi (Angie's List) Company Links Scraper](https://apify.com/babak/angi-angie-s-list-company-links-scraper) that allows to scrape links and addresses of companies by State, City, Category, and Zip Code (either separately, or simultaneously) -->


## How to use extracted Angi (Angie's List) data?
- **Market research:** Utilize Angie's List data to analyze consumer preferences, trends, and market demands. Gain insights into popular service providers and high-demand geographic areas, while identifying potential market gaps.
- **Competitive analysis:** Compare performance, customer ratings, and reviews of service providers within your industry or region using Angie's List API. Identify your competitors' strengths and weaknesses to develop effective differentiation strategies.
- **Customer feedback analysis:** Gain valuable insights by analyzing Angie's List reviews and ratings. Understand customer experiences, detect feedback patterns, and improve your products or services. Address common pain points and enhance overall customer satisfaction.
- **Lead generation:** Extract contact information from Angie's List data to identify potential leads for your business. Reach out to individuals or companies to promote your offerings, provide customized solutions, or offer discounts based on their needs.
- **Business partnerships:** Analyze Angie's List data to identify potential partners or collaborators in complementary services or industries. Establish mutually beneficial partnerships for expanding reach, offering bundled services, or cross-promoting.
- **Service improvement:** Leverage Angie's List data to identify common complaints or areas for improvement within your own business. Refine processes, enhance service quality, and deliver an exceptional customer experience.
- **Marketing and advertising:** Utilize Angie's List data to understand consumer preferences and optimize your marketing campaigns. Craft compelling messages that resonate with your target audience, highlighting your unique selling points based on the valuable insights gained.
- **Product development:** Guide your product development efforts with customer feedback and preferences extracted from Angie's List. Incorporate desired features or services into your offerings, ensuring competitiveness and meeting customer expectations.

If you would like more inspiration on how scraping Angi (Angie's List) could help your business or organization, check out our [industry pages](https://apify.com/industries).

## Is it legal to scrape Angi (Angie's List)?
Note that personal data is protected by GDPR in the European Union and by other regulations around the world. You should not scrape personal data unless you have a legitimate reason to do so. If you're unsure whether your reason is legitimate, consult your lawyers. We also recommend that you read our blog post: [is web scraping legal?](https://blog.apify.com/is-web-scraping-legal/)
