# Pilot Findings Analysis — Week 9

**Participants**: 3 (1 HTMX, 2 No-JS)
**Date range**: [2025-11-28]

---

## Quantitative Summary

### Task 1: Add New Task
| Metric          | HTMX | No-JS | KBD-only | Overall |
|-----------------|------|-------|----------|---------|
| Mean time (s)   | 12   | 15    | 32       | 19.7    |
| Success rate    | 100% | 100%  | 100%     | 100%    |
| Mean confidence | 5/5  | 5/5   | 4/5      | 4.7/5   |

**Interpretation**: High success. HTMX confidence higher (instant feedback). No-JS/KBD-only participant less sure (due to not being able to see whole screen right away and having to use KBD to scroll and view other buttons).

---

### Task 2: Edit Task
| Metric          | HTMX | No-JS | KBD-only | Overall |
|-----------------|------|-------|----------|---------|
| Mean time (s)   | 12   | 1:24  | 2:05     | 1:14    |
| Success rate    | 100% | 0%    | 0%       | 33%     |
| Mean confidence | 5/5  | 2/5   | 0/5      | 2.3/5   |

**Interpretation**: Low success. No-JS participants (P2 and P3) could not complete as edit button would not work when JS was disabled.

---

### Task 3: Deleted Task
| Metric          | HTMX | No-JS | KBD-only | Overall |
|-----------------|------|-------|----------|---------|
| Mean time (s)   | 15   | 3     | 15       | 11      |
| Success rate    | 100% | 100%  | 100%     | 100%    |
| Mean confidence | 5/5  | 5/5   | 5/5      | 5/5     |

**Interpretation**: No-JS participant performed in quicker time than P1 and P3, this could be participant-specific and most likely an outlier as P1 was HTMX and P3 was also no-JS (points to P2-specific time, rather than mode, might have to be redone or discounted).

---

## Qualitative Themes

### Theme 1: Confirmation Feedback Critical
**Evidence**: 1/3 participants mentioned seeing a confirmation (HTMX participant)
**Quotes**:
- P1 (HTMX): "I like seeing 'Task added' immediately"
- P2 (No-JS): "There isn't any confirmation for my actions"

**Design implication**: No-JS path needs explicit success message.

---

### Theme 2: Edit Button Confusing
**Evidence**: 2/3 participants hesitated to use Edit button
**Quotes**:
- P2 (No-JS) : "It should work, I clicked on the button"
- P3 (No-JS, KBD-only) : "I clicked it but it seems to just reload the page or something"

**Design implication**: Button needs to function with JS is disabled.

---

### Keyboard Navigation
- ✅ All features reachable
- ✅ Focus visible
- ⚠️ Tab order logical but Edit→Save→Cancel could be clearer
- ❌ Not all features reachable (edit button unable to be used)

---

## Prioritised Issues

Based on frequency + severity:

1. **High**: Edit button feature to work when JS is disabled
2. **Medium**: No confirmation message in no-JS path (affects 2/2 no-JS participants, low confidence)
3. **Medium**: Cancel button ambiguous (1/3 confused, but completed anyway)