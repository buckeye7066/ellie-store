# Technical Audit: Shadcn/UI ARIA Compliance Report

**Price: $49.00** · [Buy the full pack](https://buy.stripe.com/7sYdRa1aK9fLbFp7oHawo0f) · delivered as a Markdown file you can import or edit.


*Product line: technical_audit*

---

## Preview

# Technical Audit: Shadcn/UI ARIA Accessibility Compliance

## Executive Summary
This report identifies 5 high-impact ARIA implementation gaps within current community-contributed components for Shadcn/UI. These issues primarily impact screen reader navigation and keyboard interoperability.

## 1. Dialog Focus Trap Persistence
- **Issue:** In the `Dialog` primitive, dynamic content injection after the initial render fails to re-trigger the focus trap, allowing focus to escape into the underlying background document.
- **Remediation:** Implement a MutationObserver on the dialog content node to re-initialize focus trap boundaries when children update.

## 2. ComboBox ARIA-ActiveDescendant Mismatch
- **Issue:** The `Combobox` component uses `aria-activedescendant` correctly for selection, but fails to programmatically update `aria-selected` on the currently focused option element when using keyboard navigation.
- **Remediation:** Sync the `aria-selected` state with the `aria-activedescendant` ID reference in the component's state management layer.

## 3. Tabs Role Hierarchy Violation
- **Issue:** Nested `Tabs` implementations are incorrectly flattening the role hierarchy, causing parent and child tablists to announce as a single list, confusing users.
- **Remediation:** Enforce unique ID scoping for `tablist` roles and ensure child tab containers explicitly exclude `role="tablist"` if they are structurally nested.

## 4. Toast Region Live Region Politeness
- **Issue:** Toasts are being rendered as `role="status"` without an explicit `aria-live` setting, causing inconsistent announcement behavior across VoiceOver and NVDA.
- **Remediation:** Force `aria-live="polite"` on the toast viewport container regardless of the `status` role to guarantee the announcement queue.

## 5. Select Placeholder Accessibility
- **Issue:** The `Select` component's placeholder/trigger does not expose the current selection state to screen readers when no option is explicitly 'selected' by value, only by label.
- **Remediation:** Ensure the `SelectTrigger` updates the `aria-valuenow` (or equivalent descriptive label) attribute even when the value is a fallback placeholder.

---

[Buy the full pack for $49.00](https://buy.stripe.com/7sYdRa1aK9fLbFp7oHawo0f)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
