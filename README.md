# Autocomplete Search Page

A simple, self-contained HTML page that provides an autocomplete search functionality. It includes a helper tool to generate new search suggestions.

## Features

-   **Autocomplete Search:** Start typing in the search box to see a list of matching suggestions.
-   **Keyboard Navigation:** Use Arrow Up/Down and Enter/Tab to navigate and select suggestions.
-   **Suggestion Generator:** A form to easily create the code for a new suggestion item.
-   **Copy to Clipboard:** A button to copy the generated code snippet.

## Files

-   `search.html`: The main file for this tool. You can open this file directly in your web browser.
-   `suggestion.js`: This file contains the data for the search suggestions. The autocomplete feature reads from this file.

## How to Use

1.  Open the `search.html` file in a modern web browser (like Chrome, Firefox, or Edge).
2.  The page will load, and the cursor will automatically be in the search box.
3.  Start typing to see search suggestions.

## How to Add a New Suggestion

The `suggestion.js` file comes with a few examples. You can add your own by following these steps:

1.  Open the `search.html` page in your browser.
2.  Scroll to the bottom of the page to the "Add New Suggestion" form.
3.  Fill in the **Name** (the text that will appear in the suggestion list) and the **URL** (the web address to navigate to).
    -   **Note:** The URL must start with `http://` or `https://`.
4.  Click the **Copy to Clipboard** button.
5.  This will copy a JavaScript code snippet to your clipboard.
6.  Open the `suggestion.js` file in a text editor.
7.  To add your new suggestion to the existing list, you can copy the object part from the text you copied and add it to the `suggestions` array. For example:

    **If you copied this text:**
    ```javascript
    const suggestions = [
        {
            "name": "Your New Name",
            "href": "https://your.new.url.com"
        }
    ];
    ```

    **You would edit `suggestion.js` to look like this:**

    **Original `suggestion.js`:**
    ```javascript
    const suggestions = [
        {
            "name": "Google",
            "href": "https://www.google.com"
        }
    ];
    ```

    **Updated `suggestion.js`:**
    ```javascript
    const suggestions = [
        {
            "name": "Google",
            "href": "https://www.google.com"
        },
        {
            "name": "Your New Name",
            "href": "https://your.new.url.com"
        }
    ];
    ```
8.  Save the `suggestion.js` file.
9.  Refresh the `search.html` page in your browser to see your new suggestion in the autocomplete list.
