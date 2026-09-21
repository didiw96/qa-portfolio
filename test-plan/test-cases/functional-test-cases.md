# Functional Test Cases

## Booking Engine

| ID | Test Scenario | Test Data | Expected Result |
|---|---|---|---|
| TC-BE-001 | Search room availability | Valid check-in/out date | Available rooms are displayed |
| TC-BE-002 | Search with invalid date | Check-out before check-in | Validation message appears |
| TC-BE-003 | Create booking | Valid guest and room | Booking is created |
| TC-BE-004 | Create booking without guest name | Empty guest name | Required field validation appears |

## PMS

| ID | Test Scenario | Test Data | Expected Result |
|---|---|---|---|
| TC-PMS-001 | Guest check-in | Confirmed reservation | Guest is checked in |
| TC-PMS-002 | Guest check-out | Active reservation | Guest is checked out |
| TC-PMS-003 | Update room status | Room = Dirty | Room status changes to Dirty |

## POS

| ID | Test Scenario | Test Data | Expected Result |
|---|---|---|---|
| TC-POS-001 | Create order | Valid item | Order is saved |
| TC-POS-002 | Cash payment | Exact payment | Payment succeeds |
| TC-POS-003 | Cashier summary | Multiple transactions | Summary matches transactions |

## Inventory

| ID | Test Scenario | Test Data | Expected Result |
|---|---|---|---|
| TC-INV-001 | Stock In | Quantity = 10 | Stock increases by 10 |
| TC-INV-002 | Stock Out | Quantity <= stock | Stock decreases correctly |
| TC-INV-003 | Stock Out above available stock | Quantity > stock | Transaction is rejected |
| TC-INV-004 | Stock adjustment | +5 | Adjustment is recorded |

## Finance

| ID | Test Scenario | Test Data | Expected Result |
|---|---|---|---|
| TC-FIN-001 | View P&L | Valid transactions | P&L displays correct data |
| TC-FIN-002 | Night Audit | Valid business date | Business date advances |
| TC-FIN-003 | View ledger | OTA transaction | Transaction appears in correct ledger |
