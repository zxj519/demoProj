```gherkin
Feature: Beautiful Tea Shipping Costs
* Australian customers pay GST
* Overseas customers don’t pay GST
* Australian customers get free shipping for orders $100 and above
* Overseas customers all pay the same shipping rate regardless of order size

  Scenario: Calculate GST status and shipping rate
    Given the customer is from
    When the customer’s
    Then the customer
    And they are charged
    Examples:
      | country     | order total | pays GST | shipping rate          |
      | Australia   | $99.99      | Must     | Standard Domestic      |
      | Australia   | $100.00     | Must     | Free                   |
      | New Zealand | $99.99      | Must Not | Standard International |
      | New Zealand | $100.00     | Must Not | Standard International |
      | Zimbawbe    | $100.00     | Must Not | Standard International |
```
