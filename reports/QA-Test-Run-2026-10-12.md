# Belyash Farm — QA Test Report

**Date:** 2026-10-12  
**Tester:** Independent QA  
**Environment:** Linux Mint / Firefox  
**Application:** Belyash Farm Web

| Metric | Result |
|---|---|
| Total Tests | 3 |
| Passed | 2 |
| Failed | 1 |

## Test Results

| Test ID | Test Case | Status |
|---|---|---|
| TC-001 | Save / Load Persistence | PASS |
| TC-002 | JSON Backup / Restore | PASS |
| TC-003 | Invalid JSON Import | FAIL |

## Console Findings

**BUG-001 — BelyashSave Interface Error**

- Status: Reproduced
- Severity: Low (provisional)
- Reproducibility: 2/2 during initial checks
- Console message: `No interface 'BelyashSave' registered`

**BUG-002 — Missing Feedback on Invalid JSON Import**

- Status: Reproduced (2/2)
- Severity: Low (provisional)
- Invalid JSON was rejected without visible feedback.
- Existing saved profiles remained accessible.

The console error did not prevent successful restoration of saved game progress in the tested scenarios.

## Limitations

- Tests were performed in Firefox only.
- Cross-browser compatibility was not tested.
- Performance testing was not performed.

## Conclusion

Three functional test cases were executed:
two passed and one failed.

Save/load and JSON backup restoration worked
in the tested scenarios.

Invalid JSON import did not provide clear
user feedback. Existing data remained accessible.

Both reported defects require further investigation.
