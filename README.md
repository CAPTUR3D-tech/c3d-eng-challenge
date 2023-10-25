# Engineering Take Home Challenge

Hello! We're pleased to hear you're interested in joining our engineering team!

Upon review, your submission to this challenge will become the basis of a discussion on design decisions, code, and further extensions.

If any of the instructions are unclear, please feel free to reach out to us for clarification!

## Challenge

At Phoria we offer a number of services to our customers.

Your team has been tasked with building an ordering system which accepts orders for the services below (and other products/services in future). Your code should accept a JSON object with the details of the order (example provided in input.json) and should return a JSON object with computed information about the order (example provided in output.json).

Offered services and their options are as follows:

| Service          | Base unit price | Extra options                                                               |
| ---------------- | --------------- | --------------------------------------------------------------------------- |
| Photo Retouching | \$2.50          | - Background removal: + \$0.50<br />- Add Watermark: + \$0.30               |
| Floor Plan       | \$15            | - 3D layout: + \$15<br /> - Add furniture: + \$10<br /> - Add Colour: + \$5 |
| Drone video      | \$50            | - Customer branded: + \$10 <br />- Scenic footage: + \$20                   |

Your task is to create a small Ruby application (or whatever language best showcases your skills) that can complete the above task and lends itself to being extended. We expect you use automated tests to validate your solution.

## Guidelines

- This is meant to be an assignment that you spend approximately 2 to 3 hours of dedicated, focused work. Do not feel like you need to overengineer the solution with dozens of hours. We're looking for a solution that demonstrates your technical skills, design and how you approach problems.

- Think of this like an open source project. Create a repo on Github, use git effectively for source control, and use README.md to document what you built for any newcomers to your project.

- Think out loud in your submission's documentation. Document tradeoffs, the rationale behind your technical choices, or things you would do or do differently if you were able to spend more time on the project or do it again.

- As final guidelines, what we're most interested in seeing are

  1.  Code extensibility and "maintainability"
  2.  Separation of concerns
  3.  Readability
  4.  Automated testing

## Pairing with a Captur3d Developer

After completing the take-home section of this challenge, you may be invited to a pairing session with a member of the Captur3d team.

In this session we will look at extending your application with some additional features - namely discounts.

_Note: Please do not complete this section yet_, but do feel free to think about it in advance!

The business overlords have added a new marketing campaign which offers discounts to customers. The discounts will work as follows:

| Discount trigger      | Discount amount |
| --------------------- | --------------- |
| Order price over $100 | 10%             |
| Discount code used    | $10             |

Your task is to update the application to correctly account for any eligible discounts.

## Conclusion

Hopefully the above instructions are clear. If you have any questions, please feel free to reach out to us for clarification.

Good luck!
