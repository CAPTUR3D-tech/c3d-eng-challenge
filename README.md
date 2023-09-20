# Engineering Take Home Challenge

Hello! We're pleased to hear you're interested in joining our engineering team!

Upon review, your submission to this challenge will become the basis of a discussion on design decisions, code, and further extensions

## Challenge

Your team has been tasked with building an API for a service ordering system; For the first iteration, we need a "Shopping cart" endpoint that calculates the cost of services requested based on different requested options.

The system will have **discount rules** that activates on certain events, both for specific item variant and for the order as a whole. All discount rules are **cumulative**

Specific item variants cost and their discounts are as follow

| Service type             | Base unit price | Extra options | Discount rule  
| ------------------------ | --------------- | --------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Floor plan               | \$15 | - 3D: + \$15<br /> - Furnitures: + \$10<br /> - Colour: + \$5 | - 25% off over 5 items ordered (code FP_25_PERCENT_OFF) <br />- Free coloured floor plans for any new plans past the 10th (code FP_FREE_COLOUR_OVER_10) |
| Floor plan               | \$15 | - 3D: + \$15<br /> - Furnitures: + \$10<br /> - Colour: + \$5 | - 25% off over 5 items ordered (code FP_25_PERCENT_OFF) <br />- Free coloured floor plans for any new plans past the 10th (code FP_FREE_COLOUR_OVER_10) |
| Marketing video creation | \$20 | - 360: + \$25 <br />- Branding: + \$10 <br />- Fly through: + \$10 | - 20% off over 5 items ordered (code VIDEO_20_PERCENT_OFF) <br />- 50% off branded video (with branding selected) for any new videos past the 5<sup>th</sup> (code VIDEO_BRANDING_FIFTY_PERCENT_OFF) |

**Whole order discount rules** are calculated after the specific item variants rules have been calculated

| Discount rule            | Discount code                 |
| ------------------------ | ----------------------------- |
| \$20 off orders over 200 | ORDER_20_DISCOUNT_OVER_200 |
| \$40 off orders over 500 | ORDER_40_DISCOUNT_OVER_500 |

The endpoint should return a JSON response that contains

-   Order total before discount
-   Order breakdown for each object types, along with their total quantities and discount codes applied
-   Order total after discount, with order discount codes applied

We've added a couple JSON files in this repository representing the cart items needing to be calculated, which you can use to test your system

## Guidelines

-   This is meant to be an assignment that you spend approximately 2 to 3 hours of dedicated, focused work. Do not feel like you need to overengineer the solution with dozens of hours. Be biased toward quality over quantity.

-   We're relatively flexible on the tech you choose to use - our engineering team is fluent in Ruby, Node/Typescript or Python which we use day to day (pretty sure we got some Rust in there as well). Feel free to tackle this problem in a way that demonstrates your expertise of an area -- or takes you out of your comfort zone. For example, if you build Web APIs by day and want to build a frontend to the problem or a completely different language instead, by all means go for it - learning is a core competency in our group. Let us know this context in your solution's documentation.

-   Think of this like an open source project. Create a repo on Github, use git for source control, and use README.md to document what you built for the newcomer to your project.

-   Our team builds, alongside our customers and partners, systems engineered to run in production. Given this, please organize, design, test, deploy, and document your solution as if you were going to put into production. We completely understand this might mean you can't do as much in the time budget. Be biased for production-ready over features.

-   Think out loud in your submission's documentation. Document tradeoffs, the rationale behind your technical choices, or things you would do or do differently if you were able to spend more time on the project or do it again. Make sure to document how to get started with your solution in terms of setup as well!

-   As final guidelines, what we're most interested in seeing are

    1.  Code extensibility and "maintainability"
    2.  Separation of concerns
    3.  Handling of special cases
    4.  Automated testing
    5.  Error handling

Good luck!