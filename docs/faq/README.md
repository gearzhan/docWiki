# Frequently Asked Questions

Find answers to common questions about docWiki usage, troubleshooting, and best practices.

## General Questions

### What is docWiki?

docWiki is a lightweight documentation system built on Docsify that supports Markdown content and Mermaid diagrams. It's designed for creating beautiful, searchable documentation without complex build processes.

### How is docWiki different from other documentation tools?

```mermaid
quadrantChart
    title Documentation Tools Comparison
    x-axis Simple --> Complex
    y-axis Static --> Dynamic
    quadrant-1 Simple & Dynamic
    quadrant-2 Complex & Dynamic
    quadrant-3 Simple & Static
    quadrant-4 Complex & Static
    "docWiki": [0.2, 0.8]
    "GitBook": [0.6, 0.7]
    "Sphinx": [0.8, 0.5]
    "Jekyll": [0.4, 0.3]
    "VuePress": [0.7, 0.6]
    "Docsify": [0.3, 0.7]
```

### Do I need to know programming to use docWiki?

No! docWiki is designed for non-technical users. You only need to know basic Markdown syntax to create beautiful documentation.

## Setup and Installation

### How do I set up docWiki?

The setup process is straightforward:

```mermaid
flowchart TD
    A[Download docWiki] --> B[Create docs folder]
    B --> C[Add index.html]
    C --> D[Write Markdown files]
    D --> E[Start local server]
    E --> F[View documentation]
    
    style A fill:#e1f5fe
    style F fill:#c8e6c9
```

### What are the system requirements?

- Modern web browser (Chrome, Firefox, Safari, Edge)
- Local web server (Python, Node.js, or any HTTP server)
- Text editor for writing Markdown

### Can I use docWiki offline?

Yes! docWiki works completely offline once you have the files locally. No internet connection required for viewing documentation.

## Content Creation

### How do I add new pages?

1. Create a new `.md` file in the `docs` directory
2. Write your content using Markdown syntax
3. Update `_sidebar.md` to include the new page
4. Refresh your browser to see the changes

### What Markdown features are supported?

docWiki supports all standard Markdown features plus:

- Tables
- Code syntax highlighting
- Mermaid diagrams
- Custom CSS classes
- HTML elements

### How do I create diagrams?

Use Mermaid syntax within code blocks:

```mermaid
pie title Content Types in Documentation
    "Text Content" : 60
    "Code Examples" : 25
    "Diagrams" : 10
    "Images" : 5
```

## Customization

### Can I customize the appearance?

Yes! You can customize:

- Colors and themes
- Fonts and typography
- Layout and spacing
- Custom CSS styles

### How do I add a custom logo?

Add your logo to the Docsify configuration:

```javascript
window.$docsify = {
  name: 'Your Project',
  logo: '/assets/logo.png',
  // other settings...
};
```

### Can I add custom plugins?

Absolutely! docWiki supports all Docsify plugins and you can create custom ones:

```mermaid
graph LR
    A[Core docWiki] --> B[Search Plugin]
    A --> C[Mermaid Plugin]
    A --> D[Custom Plugin 1]
    A --> E[Custom Plugin 2]
    
    B --> F[Enhanced Search]
    C --> G[Diagram Rendering]
    D --> H[Analytics]
    E --> I[Comments]
```

## Troubleshooting

### Why aren't my diagrams rendering?

Common causes and solutions:

| Issue | Cause | Solution |
|-------|-------|----------|
| Blank diagram area | Syntax error | Check Mermaid syntax |
| No diagram at all | Missing plugin | Verify Mermaid plugin is loaded |
| Partial rendering | Browser compatibility | Update browser or try different one |
| Slow rendering | Complex diagram | Simplify diagram or split into parts |

### My search isn't working. What should I do?

```mermaid
flowchart TD
    A[Search not working] --> B{Plugin loaded?}
    B -->|No| C[Add search plugin]
    B -->|Yes| D{Index built?}
    D -->|No| E[Wait for indexing]
    D -->|Yes| F{Correct syntax?}
    F -->|No| G[Check search config]
    F -->|Yes| H[Clear browser cache]
    
    C --> I[Test search]
    E --> I
    G --> I
    H --> I
```

### How do I fix broken links?

1. Check file paths are correct
2. Ensure files exist in specified locations
3. Use relative paths from the docs directory
4. Test links in browser

### The site loads slowly. How can I improve performance?

Performance optimization tips:

```mermaid
mindmap
  root((Performance))
    Images
      Optimize size
      Use WebP format
      Lazy loading
    Content
      Split large files
      Remove unused content
      Minimize HTML
    Caching
      Browser cache
      Service worker
      CDN usage
    Code
      Minify JavaScript
      Reduce plugins
      Async loading
```

## Advanced Usage

### Can I integrate with version control?

Yes! docWiki works great with Git:

- Track changes to documentation
- Collaborate with team members
- Deploy automatically on commits
- Maintain version history

### How do I deploy docWiki?

Deployment options:

```mermaid
flowchart LR
    A[docWiki Source] --> B[GitHub Pages]
    A --> C[Netlify]
    A --> D[Vercel]
    A --> E[Custom Server]
    
    B --> F[Free Hosting]
    C --> F
    D --> F
    E --> G[Full Control]
```

### Can I use docWiki for team documentation?

Absolutely! docWiki is perfect for:

- API documentation
- User manuals
- Internal wikis
- Project documentation
- Knowledge bases

## Support

### Where can I get help?

- Check this FAQ first
- Browse the documentation
- Search GitHub issues
- Join our community discussions
- Contact support team

### How do I report bugs?

1. Check if the issue already exists
2. Create a minimal reproduction case
3. Include system information
4. Submit detailed bug report
5. Follow up on responses

---

*Still have questions? Feel free to reach out to our community!*