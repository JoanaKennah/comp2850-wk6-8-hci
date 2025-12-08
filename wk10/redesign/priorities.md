# Redesign Priorities — For Week 10 Lab 2

## Priority 1: Edit Inline Fails in No-JS (MUST FIX)
**Issue**: P2, P3 couldn't complete T2 in no-JS mode
**Evidence**: 33% failure rate across participants, `wk09/evidence/no-confirmation-and-no-edit-path`
**WCAG**: 2.1.1 Keyboard (A) - parity required
**Fix**: Debug no-JS edit flow, ensure PRG works
**Effort**: 1 hour

## Priority 2: No Confirmation in No-JS (SHOULD FIX)
**Issue**: P2, P3 low confidence, had to verify task added
**Evidence**: `wk09/evidence/no-confirmation-and-no-edit-path`
**WCAG**: 4.1.3 Status Messages (AA)
**Fix**: Add success message to PRG redirect (query param or session flash)
**Effort**: 1-2 hours

## Priority 3: Cancel Button Label (SHOULD FIX)
**Issue**: P2, P3 confused
**Evidence**: `wk09/evidence/cancel-button`
**WCAG**: 2.4.6 Headings and Labels (AA)
**Fix**: Change to "Cancel (discard changes)"
**Effort**: 10 minutes

## Deferred (Post-Assessment)
- Progress indicator