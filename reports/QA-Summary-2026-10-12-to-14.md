# Belyash Farm — QA Test Summary

**Period:** October 12–14, 2026  
**Environment:** Linux Mint / Firefox  
**Application:** Belyash Farm Web

## Execution Results

| Metric | Count |
|---|---|
| Total Executed | 5 |
| Passed | 4 |
| Failed | 1 |
| Documented Findings | 2 |

## Test Cases

| Test Case | Description | Result |
|---|---|---|
| TC-001 | Save / Load Persistence | PASS |
| TC-002 | JSON Backup / Restore | PASS |
| TC-003 | Invalid JSON Import | FAIL |
| TC-004 | Network Loading Without Cache | PASS |
| TC-005 | Slow Network Simulation | PASS |

## Findings

**BUG-001 — BelyashSave Interface Error**

Recurring JavaScriptBridge console error. No visible impact on save restoration was observed during the executed scenarios.

**BUG-002 — Invalid JSON Import Feedback**

Malformed JSON was not accompanied by visible error feedback. Existing saved farms remained accessible. Reproduced in two attempts.

## Network Observations

- All nine observed HTTP requests completed successfully during both unrestricted no-cache and Regular 3G runs.
- Unrestricted no-cache Network Finish: 7.10 seconds.
- Regular 3G Network Finish: 6.75 minutes.
- The game main menu was displayed successfully under both conditions.

## Limitations

Testing was conducted in Firefox on Linux Mint. The results do not establish compatibility with other browsers or operating systems.

Network timing measurements are individual observations, not a statistically representative benchmark.

## Conclusion

Four of five executed test cases passed.

Save/load, JSON backup restoration and network resource loading succeeded in the tested scenarios.

The invalid JSON import test failed because the application provided no visible error feedback.

Two findings remain documented for further investigation.
