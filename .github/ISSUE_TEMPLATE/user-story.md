---
## User Story
**As a** customer

**I need** to search products

**So that** I can quickly find items I want to buy

---

## Details and Assumptions

* Products are stored in the catalog.
* Customers can search using a product name or keyword.
* Search results should display all matching products.
* Only active products are returned in search results.

---

## Acceptance Criteria

```gherkin
Scenario: Search for a product successfully

Given I am on the product catalog page
When I enter a product name in the search box
And click the Search button
Then matching products should be displayed

Scenario: No matching products found

Given I am on the product catalog page
When I search for a product that does not exist
Then a "No products found" message should be displayed
```
