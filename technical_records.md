# Dynamic Year in Footer Implementation

## Date: 2024-07-30

## Objective:
To dynamically update the year displayed in the website footer, ensuring it always reflects the current year instead of a static value or the Jekyll build time.

## Problem:
The existing Jekyll setup used `{{ site.time | date: '%Y' }}` which updates the year only when the site is rebuilt. This resulted in the footer displaying an outdated year (e.g., 2022) if the site wasn't rebuilt annually.

## Solution Implemented:
A client-side JavaScript solution was implemented to fetch the current year from the user's browser and dynamically update the year in the footer. This approach ensures the year is always current without requiring a site rebuild.

## Changes Made:

### File: `_includes/footer.html`

**Before:**
```html
<footer class="footer-main">
    {{ site.name }} © {{ site.time | date: '%Y' }}
</footer>
```

**After:**
```html
<footer class="footer-main">
    {{ site.name }} © <span id="current-year"></span>

    <script>
        document.getElementById("current-year").textContent = new Date().getFullYear();
    </script>
</footer>
```

## Explanation:
1.  **`<span>` Element**: The original Jekyll date tag `{{ site.time | date: '%Y' }}` was replaced with an empty `<span>` element with the ID `current-year`. This provides a placeholder for the JavaScript to inject the dynamic year.
2.  **JavaScript Snippet**: A `<script>` block was added directly within the `_includes/footer.html` file.
    *   `document.getElementById("current-year")`: This selects the `<span>` element using its unique ID.
    *   `new Date().getFullYear()`: This JavaScript function creates a new `Date` object and extracts the full current year from it.
    *   `.textContent = ...`: The extracted current year is then assigned as the text content of the `<span>` element.

## Benefits:
*   **Always Up-to-Date**: The year in the footer will always display the current year for the user, regardless of when the Jekyll site was last built.
*   **No Rebuild Required**: No need to rebuild and redeploy the site annually just to update the copyright year.
*   **Simple and Efficient**: A lightweight client-side solution that is easy to maintain.

## Potential Considerations:
*   **JavaScript Dependency**: The dynamic year relies on JavaScript being enabled in the user's browser. However, for a modern website, this is generally an acceptable dependency.

## Verification:
After deployment, users should observe the current year (e.g., 2025 if the current year is 2025) displayed in the footer. 