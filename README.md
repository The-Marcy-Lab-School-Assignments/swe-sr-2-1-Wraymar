# Technical Writing Assignment

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/fullstack-curriculum/how-tos/working-with-assignments#how-to-work-on-assignments).

## Prompt 1

Do some research on semantic and non-semantic elements and share your findings. Your response should include:

- Examples of semantic and non-semantic tags
- The differences between semantic and non-semantic tags
- The benefits of using semantic tags (when possible)

### Response 1

Here’s a refined version of your text, keeping it concise and in your voice:

Semantic tags in HTML describe the type of content they contain, providing meaning to the browser and developers. For example, a <form> tag clearly indicates that its content is related to forms. These tags often include specific attributes to support structure.

Some semantic tags in HTML are:

- `<header>`
- `<table>`
- `<form>`

Non-semantic elements, like `<div>` and `<span>`, don’t convey specific meaning or describe their content.

Using semantic tags improves code readability. For instance, `<header>` is more intuitive than a `<div>` with a class like "header-content."

## Prompt 2

Do some research on accessibility. What are some ways to make your website more accessible? Explain why it is important for developers to create websites that meet accessibility standards.

### Response 2

Making your website accessible is crucial for providing a great user experience. If your site doesn’t meet accessibility standards, it might not perform well and could discourage visitors from returning.

Here are a few ways to improve accessibility:

- Alt Text for Images – Helps blind or visually impaired users by allowing screen readers to describe visual content.
- Captions and Transcripts – Beneficial for people with hearing disabilities.
- Responsive Design – Ensures your website works seamlessly across devices like computers, phones, and tablets.

## Prompt 3

It is possible to add "inline" CSS styles to our html elements using the `style` attribute like so:

```html
<p style="color: red;">hello world</p>
```

While this is possible, it is a best practice to instead write styles in a separate CSS file. Provide at least one argument for why it _might_ be considered useful to write inline styles, and then provide a more compelling argument for writing styles in a separate CSS file.

### Response 3

Pros:

Inline CSS can be useful for:

- Quick Implementation: Ideal for immediate style changes to specific elements without affecting the rest of the document.
- No Need for External Files: Eliminates the requirement for a separate stylesheet.

Major Cons:

- Difficult to Maintain: Managing styles scattered across multiple elements in the HTML can become messy.
  Increased File Size: Adds bulk to the HTML file, potentially slowing down page load times.
- Violates Separation of Concerns: Breaks the best practice of keeping HTML, CSS, and JavaScript in separate files.

## Prompt 4

Imagine you are teaching a brand new programmer a brief lesson about the `class` and `id` attributes in HTML as well as how to use them to style elements using CSS. Your lesson should have the following components:

- An explanation of the concept of "classes" and "ids" with an analogy.
- An example of the usage using an HTML code block and a CSS code block.
- An explanation of the syntax using the terms: **attribute**, **selector**

### Response 4

In HTML, IDs and classes are incredibly useful when paired with elements such as `<p>` (paragraphs), `<div>` (divisions), `<h1>` (headings), and others. An ID is used to reference a specific element and should be unique within the document. Unlike IDs, a single class can be applied to multiple elements.

To make this more understandable, imagine a large box of art supplies representing a section of our HTML. Inside this box, we might find smaller boxes containing crayons, brushes, and paint. These smaller boxes can be thought of as IDs because they reference unique items.

Within the crayon box, we may have multiple crayons in various shades of the same colors, such as reds or blues. We can group these crayons by assigning them a class of blue or red. Similarly, inside the brush box, we could organize brushes by their types, assigning classes like pointed, flat, or round. For paint, we might assign classes such as oil-paint, water-based-paint, or acrylic.

This structure allows us to organize and style our elements efficiently in HTML and CSS.

Example of how this would look as HTML code:

```html
<section>
  <h1>Crayons</h1>
  <div id="crayons">
    <div class="red">Cherry</div>
    <div class="red">Scarlet</div>
    <div class="blue">Turquoise</div>
    <div class="blue">Navy</div>
  </div>

  <h1>Brushes</h1>
  <div id="brushes">
    <div class="pointed">Pointed Brush</div>
    <div class="flat">Flat Brush</div>
    <div class="round">Round Brush</div>
  </div>
</section>
```

Your text is clear and well-structured, but a few adjustments can improve flow and clarity. Here's the revised text with a polished explanation:

Text:
When styling these IDs and classes, we can reference an ID by using the # character, followed by the ID name and curly braces. For example, to style the crayons ID, we would write:

```css

#crayons {
 /* styles */
}
To style elements with the red class, we use a period (.) before the class name, like this:

.red {
  styles
}
```

## Prompt 5

The Document Object Model (DOM) API provides functions for manipulating HTML documents. It is possible to build an entire website using only JavaScript and the DOM API, however is that the best practice?

When building a website, how can I decide which content I should write using HTML/CSS and which content I should create using the JavaScript and the DOM API?

### Response 5

Building an entire website with only JavaScript and the DOM API is possible, but it’s not the best practice. One big issue is that a single JavaScript error could stop the entire website from loading, which would ruin the user experience.

When building a website, it’s better to use HTML and CSS for static content. Write and structure your content with HTML, and make sure it’s accessible by using proper semantic tags. Keep your CSS in separate files to handle all the styling and layout.

Use JavaScript and the DOM API to handle the dynamic and interactive parts of the website. For example:

- Loading content, like search results or a user’s profile.
- Adding interactive elements, like forms, dropdowns, or modals.
- Setting up event listeners to respond to user actions like clicks or typing.

This way, you’re splitting the work between the tools that are best for each job, and you’ll end up with a website that’s easier to manage, performs better, and works well for everyone.
