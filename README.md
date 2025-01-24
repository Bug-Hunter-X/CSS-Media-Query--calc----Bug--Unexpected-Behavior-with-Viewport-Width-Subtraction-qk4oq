# CSS Media Query `calc()` Bug: Unexpected Behavior

This repository demonstrates a subtle bug related to using the `calc()` function within CSS media queries, specifically when subtracting a fixed value from `vw` (viewport width) units.  The intended behavior is to dynamically adjust styles based on a viewport width minus a certain pixel offset. However, this often doesn't work as expected across various browsers.

## Issue Description

The issue lies in the interpretation of the `calc()` function inside the media query. Some browsers may not correctly parse or apply the calculation, resulting in the media query either not triggering or applying styles incorrectly.

## Solution

The provided solution offers an alternative approach to achieve dynamic viewport width adjustments without relying on `calc()` within media queries. This avoids the browser inconsistencies and ensures more reliable behavior across different browsers.