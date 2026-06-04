# MStudio AI Design Library Specification

Version: 1.0

Status: Internal

Purpose: Design Library Generation Engine

---

# 1. Mission

This specification defines how AI should generate Design Libraries for MStudio projects.

The designer provides only high-level project inputs.

The AI is responsible for generating:

- Foundations
- Tokens
- Variables
- Component Architecture
- Documentation
- Figma Structure
- Accessibility Rules

The generated library must be scalable, maintainable, accessible and reusable.

---

# 2. Design Philosophy

Prioritize:

1. Simplicity
2. Reusability
3. Scalability
4. Accessibility
5. Developer Experience

Avoid:

- Visual complexity
- Duplicate patterns
- Hardcoded values
- One-off solutions
- Unnecessary variants

---

# 3. Mandatory Generation Rules

Always:

✓ Use Auto Layout

✓ Use Variables

✓ Use Semantic Tokens

✓ Use Component Properties

✓ Follow Atomic Design

✓ Generate Documentation

✓ Generate Responsive Rules

✓ Follow WCAG AA

Never:

✗ Use local styles

✗ Use hardcoded colors

✗ Use hardcoded spacing

✗ Use detached components

✗ Create duplicate components

---

# 4. Project Inputs

The designer provides:

## Project Information

Project Name

Industry

Platform

Library Scope

Style

Theme

Density

Border Radius Preference

---

## Brand Colors

Primary Color 500

Secondary Color 500

Optional:

Success Color 500

Warning Color 500

Error Color 500

Info Color 500

---

## Typography

Primary Font

Optional Secondary Font

---

# 5. Color Generation Rules

The designer only provides Color 500 values.

AI generates:

50

100

200

300

400

500

600

700

800

900

for every supplied color.

Generated colors must:

- Maintain hue consistency
- Maintain brand identity
- Support accessibility requirements
- Preserve visual harmony

---

# 6. Semantic Token Rules

AI must create:

## Background

Background/Primary

Background/Secondary

Background/Tertiary

Background/Inverse

---

## Text

Text/Primary

Text/Secondary

Text/Tertiary

Text/Disabled

Text/Inverse

---

## Border

Border/Subtle

Border/Default

Border/Strong

Border/Focus

---

## Actions

Action/Primary

Action/Secondary

Action/Ghost

Action/Disabled

---

## Status

Status/Success

Status/Warning

Status/Error

Status/Info

---

# 7. Typography Generation Rules

AI generates:

Display XL

Display L

Display M

Heading XL

Heading L

Heading M

Title L

Title M

Title S

Body L

Body M

Body S

Label L

Label M

Label S

Caption

Overline

For every typography token define:

- Font Family
- Size
- Weight
- Line Height
- Letter Spacing

Typography scale should be mathematically consistent.

---

# 8. Spacing System

Generate spacing tokens:

4

8

12

16

20

24

32

40

48

64

80

96

Spacing should follow an 8-point system whenever possible.

---

# 9. Radius System

Generate:

Radius/XS

Radius/S

Radius/M

Radius/L

Radius/XL

Radius/2XL

Radius/Pill

---

# 10. Elevation System

Generate:

Elevation/XS

Elevation/S

Elevation/M

Elevation/L

Elevation/XL

Every elevation token must define:

- Shadow
- Blur
- Spread
- Opacity

---

# 11. Atomic Design Hierarchy

All assets must follow:

Foundation

↓

Atom

↓

Molecule

↓

Organism

↓

Template

↓

Page

Skipping hierarchy levels is prohibited.

---

# 12. Foundations

AI must generate:

- Colors
- Typography
- Spacing
- Radius
- Elevation
- Motion
- Grid
- Breakpoints

---

# 13. Required Atoms

Icon

Avatar

Badge

Chip

Tag

Divider

Progress Indicator

Spinner

Checkbox

Radio

Switch

---

# 14. Required Molecules

Button

Input

Search

Select

Textarea

Date Picker

Tabs

Segmented Control

Breadcrumb

Pagination

---

# 15. Required Organisms

Card

Table

Navigation Bar

Sidebar

Modal

Drawer

Alert

Toast

Empty State

Stepper

Bottom Sheet

---

# 16. Component Architecture Rules

Every component must include:

Anatomy

Properties

States

Variants

Accessibility Notes

Developer Notes

Usage Guidelines

Related Components

---

# 17. State Rules

Supported states:

Default

Hover

Pressed

Focus

Disabled

Loading

Success

Error

All states must be token-driven.

---

# 18. Variant Rules

Use:

- Variables
- Properties
- Auto Layout

Avoid variant creation for:

- Width
- Text Length
- Dynamic Content
- Layout Direction

Prevent Variant Explosion.

---

# 19. Table Rules

Every generated Table must support:

- Sorting
- Selection
- Status Indicators
- Empty State

Density Modes:

Compact

Default

Comfortable

---

# 20. Form Rules

All form elements must support:

- Label
- Helper Text
- Error State
- Success State
- Disabled State

---

# 21. Accessibility Rules

Minimum:

WCAG AA

Visible Focus Indicators

Keyboard Navigation

Screen Reader Support

Accessible Color Contrast

Touch Target Compliance

---

# 22. Responsive Rules

Generate responsive behavior for:

Mobile

Tablet

Desktop

Document all breakpoint behavior.

---

# 23. Figma Rules

Every asset must:

Use Auto Layout

Use Variables

Use Component Properties

Use Semantic Tokens

Use Consistent Naming

Include Documentation

---

# 24. Figma File Structure

00 Foundations

01 Atoms

02 Molecules

03 Organisms

04 Templates

05 Pages

06 Documentation

07 Playground

99 Archive

---

# 25. Documentation Rules

Every component page must include:

Purpose

When To Use

When Not To Use

Anatomy

States

Properties

Accessibility

Examples

Developer Notes

---

# 26. Design QA Rules

Before publishing:

□ Auto Layout Used

□ Variables Applied

□ Semantic Tokens Applied

□ Naming Convention Applied

□ Accessibility Checked

□ Documentation Completed

□ Responsive Behaviour Defined

□ Developer Handoff Ready

---

# 27. Output Requirement

The generated Design Library must be immediately publishable as a Figma Library and usable by Design, Research and Development teams without additional restructuring.