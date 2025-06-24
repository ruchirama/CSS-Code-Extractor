# CSS Code Extractor

## About the App

The CSS Code Extractor is a web-based tool designed to help you compare, find, and extract specific CSS rules from a larger CSS stylesheet. Its primary purpose is to allow users to isolate desired CSS rules based on provided reference snippets, making it easier to manage, refactor, or understand complex stylesheets. This tool runs entirely in your browser, meaning no backend processing is involved and your files remain local.

## How to Work With It

The tool operates using two main inputs: "A CODES" (your reference CSS) and "B CODE" (the main CSS file you want to process).

1.  **A CODES (Reference CSS):**
    *   In the "A CODES" section, you'll find one or more text areas.
    *   Enter the specific CSS rules or snippets you are looking for into these text areas. Each distinct rule or related group of rules you want to search for can be in its own block or within the same block.
    *   You can add more "A CODE" input blocks by clicking the "+ Add Another A CODE" button or remove them using the "Remove This Code" button associated with each block.

2.  **B CODE (Upload CSS File):**
    *   In the "B CODE" section, upload the main CSS file from which you want to extract rules.
    *   You can either click the upload area to browse for your `.css` file or drag and drop the file directly onto the designated area.
    *   The tool validates the file type (must be `.css`) and size (up to 10MB).

3.  **Output File Names:**
    *   Before processing, you can specify custom filenames for the two output files:
        *   **Extracted/Found CSS Rules:** This file will contain CSS rules from your B CODE file that matched your A CODES. (Defaults to `extracted-styles.css`)
        *   **Remaining B CODE:** This file will contain CSS rules from your B CODE file that did *not* match any of your A CODES. (Defaults to `remaining-styles.css`)

4.  **Processing:**
    *   Once your A CODES are entered and your B CODE file is uploaded, click the "🚀 Extract & Compare CSS Codes" button.
    *   The tool will then parse both sets of CSS, normalize them for accurate comparison, and identify matches.

5.  **Results:**
    *   After processing, the "Results" section will display:
        *   **Summary:** An overview including the total number of A CODE rules, total B CODE rules, how many rules were matched, and how many were not found.
        *   **Found Rules:** Lists each A CODE snippet that was successfully found within the B CODE. For each match, it shows your original A CODE and the corresponding snippet from the B CODE.
            *   A "📥 Download Extracted CSS Rules" button will appear if any rules were matched, allowing you to download a CSS file containing only these found rules, formatted to maintain readability.
        *   **Not Found Rules:** Lists any A CODE snippets that were not found in the B CODE.
        *   **Remaining B CODE:** Shows a preview of the CSS from your B CODE file after all matched rules have been removed.
            *   A "📄 Download Remaining B CODE" button allows you to download a CSS file containing this remaining, unmatched CSS. If all rules were matched, this section will indicate that no rules remain.

## Advantages

*   **Targeted Extraction:** Easily isolate and extract only the specific CSS rules you need from large and complex stylesheets.
*   **Efficient Comparison:** Quickly determine which of your reference CSS rules are present or missing in a given stylesheet.
*   **Code Management & Refactoring:** Aids in cleaning up, modularizing, or refactoring CSS by helping to separate concerns or identify redundant/unused styles (when used strategically).
*   **User-Friendly Interface:** Features a straightforward interface with clear input fields, drag-and-drop file upload, and an intuitive results display.
*   **Client-Side Processing:** Operates entirely within your web browser, ensuring your CSS data remains private and processing is fast as it doesn't rely on server communication.
*   **Preserves Formatting:** The tool attempts to preserve the original formatting and spacing of the extracted and remaining CSS rules as much as possible for better readability.
