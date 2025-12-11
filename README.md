# MOBILE-AUTOMATION-TESTING
Reported by: Gajini Prasanth
Reference: Report Document 

report

Description

Two major UI/UX issues were found in the PRAM mobile app:

1. Discover screen content is clipped/unreadable

The promotional card and “NO COST Educational ERP…” section are partially cut off.
The lower content overlaps or overflows, and users cannot see the full information.
There is also no clear scroll indicator or proper spacing, leading to a poor user experience.

2. Misleading update banner in Change Language screen

A pop-up saying “Our team is racing against the clock to roll out this feature in the next version — STAY TUNED!” appears even though the feature is still under development.
This gives users a false promise and reduces trust in the app.

Steps to Reproduce
Issue 1: Discover Screen

Open the app → Go to the Discover tab.

View the promotional card and heading text (“NO COST Educational ERP…”).

Observe that the content below is partially hidden or overlapped.

Issue 2: Change Language Screen

Go to Settings → Change Language.

A modal/banner appears with a message about “next version rollout.”

This message appears even though the feature is not ready.

Actual Behavior

Discover screen content is cut off and unreadable.

Users cannot view below-the-fold information.

The “coming soon” banner appears publicly and looks like a guaranteed release promise.

Expected Behavior

Discover screen content should be fully visible and responsive across screen sizes.

Users should be able to scroll without layout overlap.

Unreleased features should not display misleading or premature banners.
A neutral message (e.g., “Feature in development”) should be used instead.

Environment

Platform: Android

App: PRAM

Version: 1.30.1

Last Update: 8 Dec 2025

Screenshots: Attached in report document 

report

Severity & Priority

Severity: Major

Priority: P1 (recommended for upcoming release)

Suggested Fixes

Layout Fix (UI)

Use responsive container heights and proper safe-area padding.

Avoid fixed heights that cause clipping.

Enable smooth vertical scrolling for long content.

Z-index & Stacking Correction

Ensure banners, cards, and headers don't overlap.

Improve UX Accessibility

Add visual scroll indicators.

Ensure promotional cards are fully readable and focusable.

Messaging Policy Update

Remove misleading “next version rollout” banners.

Only show non-committal messages like “Feature in development” if necessary.

QA Action

Add visual/regression tests for Discover & Language screens across multiple device sizes.
