✓✗# EmployeeHoverCard Component

## Overview

The EmployeeHoverCard component displays employee information in a rich preview card that appears on hover. It provides quick access to contact details, role information, and action buttons.

**Status**: Ready | **Package**: @peopleforce/ui

## Quick Links

- [Vue.js Implementation](./vue.md)
- [Rails Implementation](./rails.md)  
- [Figma Design](./figma.md)

---

## Content Displayed

- Profile picture with status
- Full name and title
- Email and phone
- Current location/office
- Department assignment
- Quick action buttons

---

## Usage

### When to Use ✓

- Display on hover over user names
- Quick employee lookup
- Contact information preview
- Team collaboration contexts

### When NOT to Use ✗

- Full profile pages
- Static employee lists
- Contact directories

---

## Properties

| Property | Type | Default | Description |
|----------|------|---------|-------------|
| `employeeId` | string | - | ID of employee to display |
| `position` | "top" \| "bottom" \| "left" \| "right" | "top" | Card position |
| `delay` | number | 500 | Hover delay in ms |

---

## Related Components

- [Avatar](../avatar/README.md) - User profile image
- [Badge](../badge/README.md) - Status indicators
