# Test Cases

The automation was tested using multiple lead scenarios to verify AI classification and conditional routing.

## Test Case 1 — High Priority Lead

### Input

A large organization actively looking for an AI marketing solution and requesting a product demonstration.

### Expected Result

* High lead score
* HIGH priority
* Sales notification triggered
* Lead recorded in processed data

### Result

Passed

---

## Test Case 2 — Medium Priority Lead

### Input

A potential customer researching AI marketing solutions and requesting additional product information.

### Expected Result

* Medium lead score
* MEDIUM priority
* Follow-up workflow triggered
* Lead recorded in processed data

### Result

Passed

---

## Test Case 3 — Low Priority Lead

### Input

A user browsing the product without an immediate purchasing requirement.

### Expected Result

* Low lead score
* LOW priority
* Lead stored without immediate sales notification

### Result

Passed

---

## Test Case 4 — Fallback Scenario

### Input

A lead containing incomplete or unexpected information.

### Expected Result

* Workflow does not silently fail
* Lead is captured by the fallback route
* Lead remains available for manual review

### Result

Passed
