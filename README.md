# Belyash Farm — Manual QA Portfolio

Manual QA testing portfolio based on a real browser-based game developed with Godot.

## Project Overview

**Application:** Belyash Farm  
**Platform:** Web (HTML5 / WebAssembly)  
**Testing Environment:** Linux Mint, Firefox  
**Testing Approach:** Manual functional testing, regression checks, negative testing and defect documentation.

**Live Application:** https://liberum-dev.github.io/belyash-farm-web/

## Test Results

| Test ID | Test Scenario | Status |
|---|---|---|
| TC-001 | Save / Load Persistence | PASS |
| TC-002 | JSON Backup / Restore | PASS |
| TC-003 | Invalid JSON Import | FAIL |

**Execution Date:** October 12, 2026

## Defects

| Bug ID | Description | Status |
|---|---|---|
| BUG-001 | JavaScriptBridge BelyashSave console error | Reproduced |
| BUG-002 | Missing user feedback on invalid JSON import | Reproduced |

## Tools

- Firefox Developer Tools — Console
- Git and GitHub
- Linux Mint
- JSON
- Markdown documentation

## Repository Structure

- `reports/` — test execution reports
- `bug-reports/` — documented defects
- `test-data/` — test fixtures
- `evidence/` — screenshots and supporting materials
- `test-cases/` — planned test-case documentation
- `checklists/` — planned testing checklists

## Next Steps

- Cross-browser testing
- Responsive web testing
- Network request inspection
- Additional negative test scenarios
- Regression testing across application versions

## Notes

This portfolio documents practical manual testing performed on a self-developed project. Test results reflect the specified environment and execution date. Findings are not presented as independent third-party product certification.
