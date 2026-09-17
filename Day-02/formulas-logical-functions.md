# Excel Day 2 — Basic Formulas & Logical Functions

## Topics Covered

- SUM()
- AVERAGE()
- COUNT()
- MIN()
- MAX()
- IF()
- AND()
- OR()

---

## 1. SUM()

**Purpose:** Adds numbers together.

**Syntax:**

`=SUM(C3:C7)`

**Example:**

If C3:C7 contains sales values, SUM adds all the values.

**Practice Result:**

Total Sales = 230000

---

## 2. AVERAGE()

**Purpose:** Finds the average of numbers.

**Syntax:**

`=AVERAGE(C3:C7)`

**Example:**

If C3:C7 contains sales values, AVERAGE calculates the mean.

**Practice Result:**

Average Sales = 46000

---

## 3. COUNT()

**Purpose:** Counts cells that contain numbers.

**Syntax:**

`=COUNT(C3:C7)`

**Practice Result:**

Number of Sales Records = 5

**Important:**

COUNT counts numeric values. It does not count normal text.

---

## 4. MIN()

**Purpose:** Finds the smallest number.

**Syntax:**

`=MIN(C3:C7)`

**Practice Result:**

Minimum Sales = 25000

---

## 5. MAX()

**Purpose:** Finds the largest number.

**Syntax:**

`=MAX(C3:C7)`

**Practice Result:**

Maximum Sales = 70000

---

## 6. IF()

**Purpose:** Checks a condition and gives one result if TRUE and another if FALSE.

**Syntax:**

`=IF(condition, value_if_true, value_if_false)`

**Example:**

`=IF(C3>=50000,"High","Low")`

**Meaning:**

If sales are greater than or equal to 50000, return "High".

Otherwise, return "Low".

### Practice Result

| Sales Rep | Sales | Status |
|---|---:|---|
| Arun | 60000 | High |
| Bala | 30000 | Low |
| Charan | 45000 | Low |
| Divya | 70000 | High |
| Esha | 25000 | Low |

**Memory Trick:**

IF = Decision

---

## 7. AND()

**Purpose:** Checks whether all given conditions are TRUE.

**Syntax:**

`=AND(condition1,condition2)`

**Example:**

`=AND(C3>=50000,B3="North")`

### Meaning

Both conditions must be TRUE:

- Sales >= 50000
- Region = North

### Practice Result

| Sales Rep | Region | Sales | Result |
|---|---|---:|---|
| Arun | North | 60000 | TRUE |
| Bala | South | 30000 | FALSE |
| Charan | North | 45000 | FALSE |
| Divya | West | 70000 | FALSE |
| Esha | South | 25000 | FALSE |

**Memory Trick:**

AND = All conditions must be TRUE

---

## 8. OR()

**Purpose:** Checks whether at least one condition is TRUE.

**Syntax:**

`=OR(condition1,condition2)`

**Example:**

`=OR(C3>=50000,B3="South")`

### Meaning

At least one of these conditions must be TRUE:

- Sales >= 50000
- Region = South

### Practice Result

| Sales Rep | Region | Sales | Result |
|---|---|---:|---|
| Arun | North | 60000 | TRUE |
| Bala | South | 30000 | TRUE |
| Charan | North | 45000 | FALSE |
| Divya | West | 70000 | TRUE |
| Esha | South | 25000 | TRUE |

**Memory Trick:**

OR = At least one condition must be TRUE

---

# Practice Dataset

| Sales Rep | Region | Sales |
|---|---|---:|
| Arun | North | 60000 |
| Bala | South | 30000 |
| Charan | North | 45000 |
| Divya | West | 70000 |
| Esha | South | 25000 |

---

# Key Results

| Analysis | Result |
|---|---:|
| Total Sales | 230000 |
| Average Sales | 46000 |
| Highest Sales | 70000 |
| Lowest Sales | 25000 |
| Number of Sales Records | 5 |

---

# Important Differences

| Function | Main Purpose |
|---|---|
| SUM() | Adds numbers |
| AVERAGE() | Finds average |
| COUNT() | Counts numeric cells |
| MIN() | Finds smallest value |
| MAX() | Finds largest value |
| IF() | Makes a decision |
| AND() | All conditions must be TRUE |
| OR() | At least one condition must be TRUE |

---

# Common Mistakes

## Mistake 1 — Using COUNT() for text

COUNT() counts numeric values, not normal text.

## Mistake 2 — Confusing AND and OR

AND requires all conditions to be TRUE.

OR requires at least one condition to be TRUE.

## Mistake 3 — Forgetting quotes for text

Correct:

`=IF(C3>=50000,"High","Low")`

Text values such as "High", "Low", "North", and "South" should be written as text.

## Mistake 4 — Using the wrong row references

When checking each employee separately, use the references from that row.

Example:

`=AND(C3>=50000,B3="North")`

Then copy the formula down.

---

# Interview Questions

## Q1. What is SUM() used for?

**Answer:**

SUM() is used to add numbers and calculate a total.

---

## Q2. What is the difference between SUM() and AVERAGE()?

**Answer:**

SUM() calculates the total, while AVERAGE() calculates the mean value.

---

## Q3. What does COUNT() do?

**Answer:**

COUNT() counts cells that contain numeric values.

---

## Q4. What is the difference between MIN() and MAX()?

**Answer:**

MIN() returns the smallest value, while MAX() returns the largest value.

---

## Q5. What is IF() used for?

**Answer:**

IF() checks a condition and returns one result when it is TRUE and another when it is FALSE.

---

## Q6. What is the difference between AND() and OR()?

**Answer:**

AND() requires all conditions to be TRUE, while OR() requires at least one condition to be TRUE.

---

# Portfolio Project

For the Sales Performance Dashboard, Day 2 formulas are used to prepare basic KPIs and business conditions.

### KPI Calculations

Total Revenue:

`=SUM(SalesRange)`

Average Sales:

`=AVERAGE(SalesRange)`

Highest Sales:

`=MAX(SalesRange)`

Lowest Sales:

`=MIN(SalesRange)`

Number of Sales Records:

`=COUNT(SalesRange)`

### Business Classification

IF() can classify sales performance.

Example:

`=IF(C3>=50000,"High","Low")`

AND() and OR() can be used to evaluate business conditions.

---

# Day 2 Revision

## Remember These

1. SUM() = Total
2. AVERAGE() = Mean
3. COUNT() = Number of numeric cells
4. MIN() = Smallest
5. MAX() = Largest
6. IF() = Decision
7. AND() = All conditions
8. OR() = At least one condition

### Quick Memory

`SUM → Total`

`AVERAGE → Average`

`COUNT → Count`

`MIN → Smallest`

`MAX → Largest`

`IF → Decision`

`AND → All`

`OR → One or more`

---

# Day 2 Practice Completed

Practiced:

- Total sales calculation
- Average sales calculation
- Highest and lowest sales
- Numeric counting
- Sales classification using IF()
- Multiple conditions using AND()
- Multiple conditions using OR()

---

# Mistake Recorded

**Mistake:** Initially used the wrong reference approach for AND() and OR().

**Correction:**

Use the current row's cell references and copy the formula down.

Example:

`=AND(C3>=50000,B3="North")`

`=OR(C3>=50000,B3="South")`

**Rule to Remember:**

One record = One row = One formula

---

# Status

Day 2 Completed
