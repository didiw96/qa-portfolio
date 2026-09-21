# Bug Reports

## BUG-001 — Cashier Summary Total Incorrect

**Module:** POS  
**Severity:** High  
**Priority:** High  
**Status:** Open

### Steps to Reproduce

1. Login to POS.
2. Create multiple cash transactions.
3. Complete the transactions.
4. Open Cashier Summary.
5. Compare the summary total with transaction totals.

### Expected Result

Cashier Summary total should match the total amount of completed transactions.

### Actual Result

Cashier Summary displays a different total.

### Evidence

Screenshot / screen recording should be attached here.

---

## BUG-002 — Night Audit Business Date Does Not Advance

**Module:** Finance  
**Severity:** Critical  
**Priority:** Critical  
**Status:** Open

### Steps to Reproduce

1. Login as authorized finance user.
2. Open Night Audit.
3. Start the closing process.
4. Complete the required steps.
5. Check the business date.

### Expected Result

Business date should advance to the next business date.

### Actual Result

Business date remains unchanged.

---

## BUG-003 — Cross-Property Data Visibility

**Module:** Security / Reporting  
**Severity:** Critical  
**Priority:** Critical  
**Status:** Open

### Steps to Reproduce

1. Login using a user assigned to Property A.
2. Open the relevant report.
3. Search or filter property data.

### Expected Result

User should only be able to access authorized property data.

### Actual Result

Data belonging to another property is displayed.

### Risk

Unauthorized users may be able to view data outside their assigned property.
