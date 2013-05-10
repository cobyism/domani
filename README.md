# Domani

Imagine if we could traverse the nodes that make up the DOM of the HTML we’re building *as we write markup*. You could do neath things like:

- Move from one node down further into the tree to select between nested nodes.
- Use CSS selector-style keyboard shortcuts such as `.` to edit the class of a node, and `#` to edit the ID.
- Edit other attributes and `data-` values for each node.
- Use vim-like keyboard shortcuts like `i` to insert/edit contents of a selected node.
- Type a shortcut for a new element, then type the tag name, and have it default to the necessary attributes.
- Hit `z` to enter an emmet/zen coding sequence and have it expanded into the navigable DOM tree.
- Export the markup.
- Drag and drop files (or even URLs) onto the tool to import the DOM and begin editing/navigating.
- Open/import DOM from GitHub blob URL or Gist URL.
- Copy/export markup to clipboard.
- Hitting `t` selects a text node as the one to add.
- Use `&` as a shortcut to bring up a selection/autocompletion of symbols/html-entities.
- Maybe one day have a side-by-side preview of the rendered markup.

Things that might be tricky from an IA perspective:

- Inline nodes. How do we split a paragraph with an inline element into the necessary 3 nodes (a text node of what is before the inline element, the inline element, and another text node of what was after the inline element) in such a way that it still feels "inline" (note: I initially presumed the tree structure would be a vertical one like markup, but that’s not necessarily a safe assumption—having a horizontal DOM node explorer could be interested itself.
- One-off things like `DOCTYPE`? Not sure if there are others that would fall into this category?
- In-file `<style>` and `<script>` tags.
- Implied nodes—i.e. HTML will almost always contain basic meta tags and so forth.
- Implementing a modal system for navigation versus insertion (horizontal cursor/caret for a vertical node structure).

It would be amazing if the demo was the project opening up it’s own DOM for you to navigate. Just sayin’.
