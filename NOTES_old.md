# Static Site Generators for GitHub Pages

GitHub Pages supports several static site generators, with **Jekyll** being the default. However, you can use others by building the site locally or using GitHub Actions.

## 1. Jekyll (Default for GitHub Pages)
- Built into GitHub Pages, no extra setup required.
- Supports **Markdown, Liquid templates, and themes**.
- Can use plugins if built locally.
- 📖 [Jekyll Documentation](https://jekyllrb.com/)

## 2. Hugo
- Fast and lightweight.
- Written in **Go**, does not require Ruby.
- Needs to be built before deploying to GitHub Pages.
- 📖 [Hugo Documentation](https://gohugo.io/)

## 3. MkDocs
- Great for **documentation sites**.
- Supports **Markdown** with a simple configuration.
- Can be used with themes like **Material for MkDocs**.
- 📖 [MkDocs Documentation](https://www.mkdocs.org/)

## 4. Docusaurus
- Developed by **Facebook**, optimized for documentation.
- Uses **React components**.
- Markdown-based but allows **interactive React elements**.
- 📖 [Docusaurus Documentation](https://docusaurus.io/)

## 5. Pelican
- **Python-based**, useful for blogs and scientific sites.
- Supports **reStructuredText and Markdown**.
- 📖 [Pelican Documentation](https://docs.getpelican.com/)

## 6. Gatsby
- **React-based**, highly customizable.
- Can be used with **Markdown, APIs, or CMS**.
- 📖 [Gatsby Documentation](https://www.gatsbyjs.com/)

## 7. Next.js (with Static Export)
- **React-based**, great for hybrid static and server-rendered pages.
- Needs to be built before deployment.
- 📖 [Next.js Documentation](https://nextjs.org/)

## Deployment Considerations
- **Jekyll** works directly with GitHub Pages.
- **Hugo, MkDocs, Pelican, Gatsby, and Next.js** require a **build step** before deployment (e.g., using **GitHub Actions** or a **CI/CD pipeline**).
- **Docusaurus** also requires pre-building.

Would you like recommendations based on your project type? 🚀

<br>
<br>

------
# Recommended Static Site Generator for Your Research Website

Since you are a **senior researcher** and need a structured website with a menu including:
- **Home**
- **Publications**
- **Teaching**
- **Software**
- **Projects**
- **Popularization**
- **Contact**

I recommend **Jekyll** or **MkDocs**, depending on your preference:

## 🔹 Option 1: Jekyll (Best for Customizable Websites)
- **Pros**:
  - Integrated with **GitHub Pages** (no extra setup needed).
  - Supports themes (e.g., [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/)).
  - Allows for custom layouts using **Markdown + Liquid**.
  - Can include **LaTeX support** for mathematical content.

- **Cons**:
  - Requires some setup if using advanced themes.
  - Plugins need a local build process.

📖 **Getting Started**: [Jekyll Documentation](https://jekyllrb.com/)


## 🔹 Option 2: MkDocs (Best for Simplicity & Documentation Style)
- **Pros**:
  - Easy to set up with **Markdown**.
  - Great for organizing research publications and projects.
  - Can use **Material for MkDocs**, which is highly customizable.
  - **Supports LaTeX natively** for mathematical content.

- **Cons**:
  - Requires **GitHub Actions** to deploy on GitHub Pages.
  - Less flexible for advanced layouts compared to Jekyll.

📖 **Getting Started**: [MkDocs Documentation](https://www.mkdocs.org/)

---

## 🚀 Next Steps
Would you like:
- A **pre-configured template** for one of these options?
- Guidance on **customizing themes**?
- Help setting up **GitHub Actions** for deployment?

Let me know, and I’ll prepare the necessary files! 🎯


<br>
<br>

-----

# 📖 Introduction to MkDocs

## 🔹 What is MkDocs?
**MkDocs** is a **static site generator** that builds websites using **Markdown**. It is simple, fast, and ideal for documentation-style websites, making it a great choice for researchers.

## 🔹 Key Features
- **Markdown-based**: Write content in `.md` files.
- **Fast & lightweight**: Generates a static website quickly.
- **Theming support**: Use themes like [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).
- **Search functionality**: Comes with built-in full-text search.
- **Supports LaTeX**: Ideal for research publications.

## 🔹 Installation
MkDocs requires Python. Install it with:

```sh
pip install mkdocs
```

For the **Material theme** (highly recommended):

```sh
pip install mkdocs-material
```

## 🔹 Creating a New Site
Run the following commands:

```sh
mkdocs new my-site
cd my-site
```

This will create a project structure like:

```
my-site/
│── docs/            # Markdown files go here
│   ├── index.md     # Home page
│── mkdocs.yml       # Configuration file
```

## 🔹 Running the Development Server
Preview your site locally:

```sh
mkdocs serve
```

Then visit: [http://127.0.0.1:8000](http://127.0.0.1:8000)

## 🔹 Building and Deploying
To generate static files:

```sh
mkdocs build
```

To deploy on **GitHub Pages**:

```sh
mkdocs gh-deploy
```

## 🔹 Customization
Edit `mkdocs.yml` to configure the site, for example:

```yaml
site_name: "My Research Website"
theme:
  name: "material"
nav:
  - Home: index.md
  - Publications: publications.md
  - Teaching: teaching.md
  - Software: software.md
  - Projects: projects.md
  - Popularization: popularization.md
  - Contact: contact.md
```

---

## 🚀 Next Steps
Would you like a **customized MkDocs setup** for your research website? Let me know, and I can generate the files for you! 🎯


<br>
<br>

----

# 📖 Introduction to MkDocs

## 🔹 What is MkDocs?

**MkDocs** is a **static site generator** that builds websites using **Markdown**. It is simple, fast, and ideal for documentation-style websites, making it a great choice for researchers.

## 🔹 Key Features

- **Markdown-based**: Write content in `.md` files.
- **Fast & lightweight**: Generates a static website quickly.
- **Theming support**: Use themes like [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).
- **Search functionality**: Comes with built-in full-text search.
- **Supports LaTeX**: Ideal for research publications.

## 🔹 Installation

MkDocs requires Python. Install it with:

```sh
pip install mkdocs
```

For the **Material theme** (highly recommended):

```sh
pip install mkdocs-material
```

## 🔹 Creating a New Site

Run the following commands:

```sh
mkdocs new my-site
cd my-site
```

This will create a project structure like:

```
my-site/
│── docs/            # Markdown files go here
│   ├── index.md     # Home page
│── mkdocs.yml       # Configuration file
```

## 🔹 Running the Development Server

Preview your site locally:

```sh
mkdocs serve
```

Then visit: [http://127.0.0.1:8000](http://127.0.0.1:8000)

## 🔹 Building and Deploying

To generate static files:

```sh
mkdocs build
```

To deploy on **GitHub Pages**:

```sh
mkdocs gh-deploy
```

## 🔹 Customization

### 📌 Basic Configuration

Edit `mkdocs.yml` to configure the site, for example:

```yaml
site_name: "My Research Website"
theme:
  name: "material"
nav:
  - Home: index.md
  - Publications: publications.md
  - Teaching: teaching.md
  - Software: software.md
  - Projects: projects.md
  - Popularization: popularization.md
  - Contact: contact.md
```

### 🎨 Customizing the Theme

#### Using a Built-in Theme

Modify `mkdocs.yml` to specify a theme:

```yaml
theme:
  name: "readthedocs"
```

Other available themes include `mkdocs` (default), `readthedocs`, and `material` (most customizable).

#### Customizing the Material Theme

If using `material`, you can customize colors, fonts, and layouts:

```yaml
theme:
  name: "material"
  palette:
    primary: "blue"
    accent: "orange"
  font:
    text: "Roboto"
    code: "Fira Code"
  features:
    - navigation.tabs
    - search.highlight
    - content.code.annotate
```

#### Adding a Logo and Favicon

```yaml
theme:
  name: "material"
  logo: "assets/logo.png"
  favicon: "assets/favicon.ico"
```

Ensure your images are in the `docs/assets/` folder.

### 🌟 Adding Custom CSS

To further style your site, create a `custom.css` file inside `docs/assets/` and reference it in `mkdocs.yml`:

```yaml
extra_css:
  - assets/custom.css
```

Example `custom.css`:

```css
h1 {
    color: #003366;
}
```

### 🏗️ Extending Functionality with Plugins

Enable **MkDocs plugins** by adding to `mkdocs.yml`:

```yaml
plugins:
  - search
  - mkdocs-material
```

### 🏠 Custom Homepage Design

To create a **custom homepage**, edit `docs/index.md` and format it using Markdown:

```md
# Welcome to My Research Website

![My Logo](assets/logo.png)

## 📌 About Me
I am a senior researcher working on various projects in computational science.

## 🔬 Research Interests
- Data Science
- Machine Learning
- Scientific Computing

## 📚 Latest Publications
- **Title 1** - Journal, Year
- **Title 2** - Conference, Year
```

For advanced layouts, use **Material theme features** like grids and callouts:

```md
::: {.grid}

## Column 1
Some content here.

## Column 2
More content here.

:::
```

### ✍️ Enabling LaTeX for Math Equations

To **enable LaTeX support**, add this to `mkdocs.yml`:

```yaml
markdown_extensions:
  - pymdownx.arithmatex:
      generic: true
extra_javascript:
  - https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-AMS-MML_HTMLorMML
```

Now, you can use LaTeX in your `.md` files:

```md
$$E = mc^2$$
```

Or inline:

```md
Einstein's equation is $E = mc^2$.
```

### 🎭 Custom Layouts

To create more **advanced layouts**, use Material theme's built-in **grid system** and **admonitions**:

#### Two-Column Layout

```md
::: grid

## Left Column {.cell}
- Feature 1
- Feature 2

## Right Column {.cell}
![Example Image](assets/example.png)

:::
```

#### Callouts for Highlighted Content

```md
!!! info "Research Highlight"
    Our latest paper introduces a novel algorithm for scientific computing.
```

#### Cards for Organizing Information

```md
::: grid

### 📖 Publications {.card}
[Read more](publications.md)

### 🖥️ Software {.card}
[Explore tools](software.md)

### 📡 Projects {.card}
[View projects](projects.md)

:::
```

For more customization, see [MkDocs Material Docs](https://squidfunk.github.io/mkdocs-material/).

---

## 🚀 Next Steps

Would you like further customization, such as **interactive elements or embedding Jupyter notebooks**? Let me know! 🎯


# Embedding Jupyter Notebooks in MkDocs

To embed Jupyter notebooks on your website using MkDocs, follow these steps:

## 1. Convert Notebooks to HTML or Slides

First, convert your Jupyter notebooks into a format that MkDocs can easily display, such as HTML or reveal.js slides. Use `nbconvert` for conversion:

### Convert to HTML:
```bash
jupyter nbconvert --to html your_notebook.ipynb
```

### Convert to Slides:
```bash
jupyter nbconvert --to slides your_notebook.ipynb
```

This will generate an HTML file you can embed.

## 2. Serve Notebooks Using `nbviewer` (Optional)

If you want to directly display the notebooks without converting them, you can host them on `nbviewer`. You just need to provide the link to the notebook hosted on GitHub or a similar platform.

## 3. Embedding with MkDocs

After converting the notebook to HTML or slides, place the HTML file in your MkDocs project directory (e.g., in a folder like `docs/notebooks/`).

In your MkDocs `.md` file (e.g., under the `Projects` or `Teaching` section), you can embed the notebook by linking to or including the HTML content. Here are some examples:

### Example: Link to the Notebook
```markdown
[View the Jupyter Notebook](notebooks/your_notebook.html)
```

### Example: Embed as an iframe
```markdown
<iframe src="notebooks/your_notebook.html" width="100%" height="600px"></iframe>
```

## 4. Including LaTeX and Code Output

- **LaTeX**: MkDocs supports LaTeX rendering with the `pymdown-extensions` plugin, which you can configure in your `mkdocs.yml`.
- **Code Output**: If you want code execution directly on the page, you would need to integrate with tools like Binder or Google Colab, which can allow users to run notebooks interactively.

## 5. Automating with GitHub Actions (Optional)

If you're frequently updating notebooks, you can automate the conversion process using GitHub Actions so that new notebooks are automatically converted and deployed.


<br>
<br>
-----


# Templates in MkDocs and How to Adapt Them

MkDocs uses themes to control the look and feel of your website. A theme consists of HTML templates, static assets (CSS, JS), and other settings that define the appearance. The default theme, `mkdocs`, can be customized, or you can switch to other available themes, such as `material`.

## 1. Using MkDocs Templates

MkDocs templates are based on the Jinja2 templating engine. This allows you to create custom layouts by modifying the base HTML templates. Here's how to adapt them:

### Customizing the `mkdocs.yml` Configuration

You can specify the theme in your `mkdocs.yml` file. For example, to use the `material` theme:

```yaml
theme:
  name: 'material'
  custom_dir: 'theme'
```

This tells MkDocs to use the `material` theme and look for custom templates in the `theme/` directory.

### Modifying Templates

- Templates are located in the theme's `templates/` directory. If you want to override them, copy the relevant template from the theme directory and place it in your own `theme/` directory in your project.
- Common templates you may want to modify include:
  - `base.html`: The main HTML structure.
  - `index.html`: The template for the homepage.
  - `page.html`: The template for individual pages.

### Example: Modifying `base.html`

To modify the navigation or layout, you can edit `base.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>{{ page.title }} - {{ site_name }}</title>
  <link rel="stylesheet" href="{{ base_url }}assets/stylesheets/main.css">
</head>
<body>
  <header>
    <nav>
      <ul>
        <li><a href="{{ base_url }}">Home</a></li>
        <li><a href="{{ base_url }}about">About</a></li>
      </ul>
    </nav>
  </header>
  <main>
    {{ content }}
  </main>
</body>
</html>
```

You can add custom navigation, styles, or scripts as needed.

## 2. Creating Custom Pages and Layouts

In addition to the templates, you can also create custom pages with custom layouts. For example, you could create a new `projects.html` template for a page dedicated to projects.

```html
{% extends "base.html" %}

{% block content %}
  <h1>Projects</h1>
  <ul>
    <li><a href="project1.html">Project 1</a></li>
    <li><a href="project2.html">Project 2</a></li>
  </ul>
{% endblock %}
```

This will extend the base template, allowing you to add custom content for your project page.

## 3. Customizing Static Assets

If you need to customize the appearance, you can modify or add static assets such as CSS and JavaScript. Place these files in the `docs/assets/` directory or a custom `static/` directory. Then, reference them in the templates:

```html
<link rel="stylesheet" href="{{ base_url }}assets/stylesheets/custom.css">
```

## 4. Using Plugins

MkDocs supports several plugins to enhance functionality. For example, the `mkdocs-macros-plugin` allows you to create custom macros that can be used throughout your templates.

### Example: Creating a Macro

In your `mkdocs.yml`:

```yaml
plugins:
  - search
  - macros:
      macros_dir: macros/
```

Then, define your macros in the `macros/` directory and use them in templates:

```html
{{ my_macro('Custom Content') }}
```

<br>
<br>

----

# Pre-configured MkDocs Template with Custom Menu

To create a custom MkDocs template with your specific menu, you can modify the `mkdocs.yml` configuration and the theme templates. Below, I'll show you how to configure MkDocs with a pre-configured template that includes the menu sections you've mentioned: Home, Publications, Teaching, Software, Projects, Popularization, and Contact.

## 1. Define the Menu in `mkdocs.yml`

First, you need to configure the menu items in the `mkdocs.yml` file. You can set up a navigation structure like this:

### Example `mkdocs.yml`:

```yaml
site_name: My Research Website

theme:
  name: material  # You can use any theme you prefer
  custom_dir: theme  # Custom theme directory (optional)

nav:
  - Home: index.md
  - Publications: publications.md
  - Teaching: teaching.md
  - Software: software.md
  - Projects: projects.md
  - Popularization: popularization.md
  - Contact: contact.md

extra_css:
  - css/custom_styles.css  # Add custom styles if needed
extra_javascript:
  - js/custom_scripts.js  # Add custom JavaScript if needed
```

In this example, the `nav` section defines the top-level menu items of your site, each pointing to a respective Markdown page. You can add additional nesting within the menu if needed.

## 2. Using a Pre-configured Template

If you are using the `material` theme (a popular MkDocs theme), it comes pre-configured with a clean, modern design and supports custom navigation menus. You don’t need to create a custom template unless you want to make significant changes to the layout or other elements.

### Theme Customization

If you want to make customizations to the theme (e.g., change colors, fonts, or layout), you can create a `theme` directory and override the default templates.

Here’s how to extend the `material` theme with a custom header and footer, for instance:

1. **Create a `theme` Directory**: In your MkDocs project, create a `theme` folder.
2. **Override Templates**: Copy the default template files from the theme (like `base.html` or `nav.html`) and place them in the `theme` folder. You can find the default theme files in the installed MkDocs package (in the `mkdocs-material` directory).
3. **Update `mkdocs.yml`**: Add the following to the `mkdocs.yml`:

```yaml
theme:
  name: material
  custom_dir: theme  # Point to your custom theme directory
```

## 3. Customizing Navigation with `mkdocs.yml`

You can add further customization to the navigation or individual pages. For example, to make the Publications page show a list of recent publications, you might add a custom section in your `publications.md` page like this:

### Example `publications.md`:
```markdown
# Publications

## Recent Publications

- **Title of Paper 1** - Journal, Year
- **Title of Paper 2** - Conference, Year
- **Title of Paper 3** - Journal, Year
```

This can be further styled and enhanced with custom CSS or JavaScript to make it more interactive or visually appealing.

## 4. Example Directory Structure

Your project directory might look something like this:

```
my_project/
├── docs/
│   ├── index.md
│   ├── publications.md
│   ├── teaching.md
│   ├── software.md
│   ├── projects.md
│   ├── popularization.md
│   └── contact.md
├── theme/
│   ├── base.html
│   ├── nav.html
│   └── extra.css
├── mkdocs.yml
```

## Conclusion

This setup provides a clean, pre-configured template with a simple menu structure. You can further customize the theme, add content to the pages, and use custom CSS/JavaScript to adjust the look and feel of your site. The `material` theme offers a solid foundation for this, and the configuration in `mkdocs.yml` allows for easy adaptation to your needs.

<br>
<br>
---

# Customized MkDocs Setup with Menu and Features

To set up a customized MkDocs website, we will focus on adapting the structure, navigation, and appearance to match your requirements. Here's how to customize MkDocs with your specific menu (Home, Publications, Teaching, Software, Projects, Popularization, and Contact) and make additional customizations.

## 1. `mkdocs.yml` Configuration

In your `mkdocs.yml` file, you will define the structure, theme, and navigation for your site. Here's how to set up the configuration:

### Example `mkdocs.yml`:

```yaml
site_name: My Research Website
site_url: https://my-research-website.com

theme:
  name: material  # Use the Material theme for a modern, clean layout
  custom_dir: theme  # Directory for custom theme files

nav:
  - Home: index.md
  - Publications: publications.md
  - Teaching: teaching.md
  - Software: software.md
  - Projects: projects.md
  - Popularization: popularization.md
  - Contact: contact.md

extra_css:
  - css/custom_styles.css  # Link to custom CSS if needed
extra_javascript:
  - js/custom_scripts.js  # Link to custom JavaScript if needed

markdown_extensions:
  - toc:
      permalink: true  # Table of Contents with permalinks for easy navigation
  - codehilite:  # Syntax highlighting for code blocks
  - pymdownx.details:  # Allows collapsible sections (great for FAQs or long lists)

plugins:
  - search  # Enable the built-in search functionality
  - awesome-pages  # Automatically generate a nice sidebar for navigation
```

### Explanation of Fields:
- **`site_name`**: The name of your site, which will appear in the header and metadata.
- **`nav`**: This defines the menu structure for your site with links to each of your content pages.
- **`theme`**: The `material` theme is used here. It's a responsive theme with modern features, like a sticky sidebar and collapsible navigation.
- **`extra_css`** and **`extra_javascript`**: Link to custom files for further styling and functionality.
- **`markdown_extensions`**: Extensions like `toc` for a table of contents, `codehilite` for syntax highlighting, and `pymdownx.details` for collapsible content sections.
- **`plugins`**: The search plugin for indexing your content and `awesome-pages` for automatic sidebar generation.

## 2. Directory Structure

Your project directory should look like this:

```
my_project/
├── docs/
│   ├── index.md           # Home page
│   ├── publications.md    # Publications page
│   ├── teaching.md        # Teaching page
│   ├── software.md        # Software page
│   ├── projects.md        # Projects page
│   ├── popularization.md  # Popularization page
│   └── contact.md         # Contact page
├── theme/                 # Custom theme files (if needed)
│   ├── base.html          # Custom base template
│   ├── nav.html           # Custom navigation
│   └── extra.css          # Custom CSS styles
├── mkdocs.yml             # MkDocs configuration file
└── requirements.txt       # Python dependencies (for MkDocs, plugins)
```

### Example Content for Pages:

#### `index.md` (Home Page):
```markdown
# Welcome to My Research Website

This is the homepage of my research website. Here, you will find information about my publications, teaching materials, software tools, and more.

## About Me

I am a senior researcher focused on various scientific and technological advancements.
```

#### `publications.md` (Publications Page):
```markdown
# Publications

## Recent Publications

- **Paper Title 1** - Published in Journal XYZ, 2024
- **Paper Title 2** - Presented at Conference ABC, 2023

[Read More](https://example.com)
```

## 3. Customizing the Theme

If you'd like to customize the appearance of the site further, you can override the default Material theme templates by adding custom files to the `theme` directory.

For example, you can:
- Modify `base.html` to adjust the header, footer, or page layout.
- Adjust the sidebar or navigation by modifying `nav.html`.
- Add custom CSS in `extra.css` to style your pages as needed.

### Example of Custom CSS (`theme/extra.css`):

```css
/* Custom styles for the header */
header {
    background-color: #4CAF50;
    padding: 20px;
    color: white;
}

/* Style the navigation bar */
nav {
    background-color: #333;
}

nav a {
    color: white;
    padding: 14px 20px;
    text-decoration: none;
}

nav a:hover {
    background-color: #ddd;
    color: black;
}
```

## 4. Additional Features

- **Search**: The built-in search functionality allows users to search for specific content on your website.
- **Table of Contents (TOC)**: Automatically generated for each page with `markdown_extensions.toc`.
- **Syntax Highlighting**: With the `codehilite` extension, you can add syntax-highlighted code blocks.

Example of a syntax-highlighted code block:
```python
def my_function():
    print("Hello, World!")
```

- **Collapsible Sections**: Using `pymdownx.details`, you can create collapsible sections for FAQs or long lists.

Example of a collapsible section:
```
markdown
### FAQ

<details>
<summary>What is MkDocs?</summary>
MkDocs is a static site generator that's geared towards project documentation.
</details>
```

## Conclusion

This setup provides a fully customized MkDocs project with a clean and modern navigation menu. You can further enhance your site with additional styling, interactive features, and easy-to-manage content.


