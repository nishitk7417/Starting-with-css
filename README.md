QUESTION-1:Create a simple page with some div tags and show different ways to add CSS as well as what happens
when you target the same elements with inline, internal, and external CSS. Also, utilize comments in the
project where required.
Explanation:
Internal CSS and External CSS both target elements with the class .box. The styles defined in the external CSS file (styles.css) will override those defined in the internal CSS block because of the cascading nature of CSS, where later rules take precedence.
Inline CSS on the first div overrides both internal and external styles for that specific div, demonstrating that inline styles have the highest specificity.
Summary:
Inline CSS: Highest specificity, overrides internal and external CSS.
Internal CSS: Applies styles to elements within the same HTML file, but can be overridden by external CSS.
External CSS: Applied using a separate CSS file, can be overridden by inline styles due to specificity rules.

QUESTION-2:Build an HTML page with multiple paragraphs, each assigned a unique class name. Write CSS rules using class selectors to apply distinct styling to each paragraph. Follow the BEM naming convention and explain how you've named the classes.
Explanation:
Each paragraph (<p>) is placed inside a <div> with the class paragraph. This is the block in BEM terminology.
Each paragraph has a unique class name to style it distinctly:
.paragraph__text: This is the element inside the block paragraph. It styles the first paragraph.
.paragraph__text--highlighted: This uses a modifier (--highlighted) to modify the element style. It styles the second paragraph differently.
.paragraph__text--large: Another modifier (--large) to style the third paragraph differently.

Explanation:
Base styling (paragraph): Applies basic styling to each paragraph container (div) to provide consistent spacing and border.
Element styling (paragraph__text): Defines common styles for the paragraph text (<p>) inside each paragraph block.
Modifiers (--highlighted and --large): Modify the styles of the paragraph text (paragraph__text) when combined with the respective modifiers.

Naming Convention (BEM):
Block: .paragraph - Represents the component as a whole.
Element: .paragraph__text - Represents an element inside the block (the paragraph text).
Modifier: .paragraph__text--highlighted and .paragraph__text--large - Modifies the element's style to convey specific variations.

Summary:
Using the BEM naming convention helps organize and structure CSS classes in a clear and meaningful way:
Blocks represent standalone components (paragraph).
Elements are parts of a block (paragraph__text).
Modifiers change the appearance or behavior of elements (paragraph__text--highlighted, paragraph__text--large).
This approach enhances maintainability and readability of CSS, making it easier to understand the relationships and styles applied to different parts of the HTML structure.

QUESTION-3:Develop an HTML form with various input elements. Use CSS to style the form, including setting
background colors for input fields. Create a custom color palette for the form elements, and demonstrate how to apply opacity to one of the form sections.
Explanation:
The form contains various input elements such as text input, email input, textarea, number input, color picker, and checkbox.
Each input element is wrapped in a <div> with the class form-section to facilitate styling.
The last <div> with the class form-section has inline CSS (style="opacity: 0.8;") to demonstrate applying opacity to a section of the form.
Global styles: Set the body background color and overall padding.
Form container: Styled to have a centered layout with padding, background color, border radius, and box shadow for a card-like appearance.
Form styling: Utilizes CSS grid for layout (display: grid) and adds gaps between grid items (gap property).
Form sections: Each .form-section is styled with grid layout to align labels and inputs vertically.
Input styling: All input elements (input[type="text"], input[type="email"], etc.) have consistent styling with padding, border, border radius, and a light background color.
Checkbox styling: Adjusted width to fit content (width: auto;).
Button styling: Styled with a green background color (#4CAF50), white text, rounded corners, and hover effect.
Custom Color Palette:
In the provided CSS, you can replace colors such as #4CAF50, #45a049, #f0f0f0, #fff, #f9f9f9, #ccc, and others with your custom color palette to match your design preferences.
Applying Opacity:
The <div> with the class form-section and inline style style="opacity: 0.8;" demonstrates how to apply opacity to a specific section of the form. This makes the contents of that section slightly transparent.

Summary:
This example demonstrates how to create a styled HTML form using CSS, including customizing colors and applying opacity. The form structure is organized using <div> elements for each section, making it easy to apply styles uniformly and apply specific styling effects where needed.
