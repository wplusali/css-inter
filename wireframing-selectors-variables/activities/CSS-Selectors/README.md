# 📖 Implement an Icon for Downloadable Style Sheets

Work with a partner to implement the following user story:

* As a user, I want to see an icon next to every `<a>` element that has a link to a downloadable CSS file in its `href` attribute.

## Instructions

* Add a 📝 emoji to any link to a CSS file.
  * Should be added only using CSS


Your web application should look like the following image once complete:

![The updated page shows an emoji next to each link that takes you to a CSS file.](./images/01-selector-complete.png)

### 💡 Hints

* How can you target a file type by its file extension (i.e., `.css`, `.html`, `.md`, etc.)?

Refer to the following documentation: 

[MDN Web Docs on attribute selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/Attribute_selectors)

### 🏆 Bonus

If you have completed the activity and want to further your knowledge, work through the following challenge with your partner:

### How do selectors affect CSS performance? ###

Use [Google](https://www.google.com) or another search engine to research this.

CSS selectors can indeed impact the performance of a webpage, particularly in how quickly the browser can render the page. The effect of CSS selectors on performance typically becomes more noticeable in very large or complex documents with a significant amount of CSS. Here's how different types of selectors can affect performance:

1. **Simple vs. Complex Selectors**: 
   - **Simple selectors** (e.g., tag, class, or ID selectors) are generally fast because they are straightforward for the browser to parse and apply.
   - **Complex selectors** (e.g., descendant selectors like `div p`, child selectors like `div > p`, or sibling selectors like `div + p`) can be slower because they require more work from the browser to evaluate relationships between elements.

2. **Universal Selectors**:
   - The universal selector (`*`) can be performance-intensive, particularly if used with complex rules or on large documents, as it applies to every element in the DOM.

3. **Attribute Selectors**:
   - Attribute selectors (e.g., `[attribute="value"]`) are generally slower than class or ID selectors, as the browser needs to inspect each element's attributes.

4. **Pseudo-Classes and Pseudo-Elements**:
   - Pseudo-classes (e.g., `:hover`, `:nth-child()`) and pseudo-elements (e.g., `::before`, `::after`) can have varying impacts on performance depending on their specificity and how they are used.

5. **Selector Specificity**:
   - Highly specific selectors (e.g., deeply nested selectors or those with multiple classes/IDs) can be slower to match because the browser has to perform more checks.

6. **Quantity of Selectors**:
   - The sheer number of selectors can impact performance. A large stylesheet with thousands of rules will take longer for the browser to parse and apply.

7. **Render-Blocking CSS**:
   - CSS that is render-blocking (styles that must be loaded before the page can be rendered) can delay the initial rendering of the page.

### Best Practices for CSS Performance:

- **Use Class Selectors**: They are generally more efficient than other types of selectors.
- **Minimize Depth**: Avoid deeply nested selectors.
- **Avoid Universal Selectors**: Especially in complex rules or on large pages.
- **Be Specific, But Not Overly So**: Overly specific selectors can slow down performance.
- **Optimize Render-Blocking CSS**: Inline critical CSS and defer non-critical styles.
- **Clean and Organize**: Regularly refactor CSS to remove unused rules and reduce file size.

In modern web development, the impact of CSS selectors on performance is usually minimal, especially with the efficiency of modern browsers and the small size of typical CSS files. However, for large-scale applications with extensive stylesheets, these considerations become more critical.
---
© 2023 edX Boot Camps LLC. Confidential and Proprietary. All Rights Reserved.