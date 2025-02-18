# Générateurs de Sites Statics pour GitHub Pages

GitHub Pages prend en charge plusieurs générateurs de sites statiques, **Jekyll** étant celui par défaut. Toutefois, vous pouvez utiliser d'autres générateurs en créant le site localement ou en utilisant GitHub Actions.

## 1. Jekyll (Par défaut pour GitHub Pages)
- Intégré directement dans GitHub Pages, aucune configuration supplémentaire nécessaire.
- Supporte **Markdown, les modèles Liquid, et les thèmes**.
- Permet d'utiliser des plugins si construit localement.
- 📖 [Documentation de Jekyll](https://jekyllrb.com/)

## 2. Hugo
- Rapide et léger.
- Écrit en **Go**, ne nécessite pas Ruby.
- Doit être construit avant de pouvoir être déployé sur GitHub Pages.
- 📖 [Documentation de Hugo](https://gohugo.io/)

## 3. MkDocs
- Idéal pour les **sites de documentation**.
- Supporte **Markdown** avec une configuration simple.
- Peut être utilisé avec des thèmes comme **Material for MkDocs**.
- 📖 [Documentation de MkDocs](https://www.mkdocs.org/)

## 4. Docusaurus
- Développé par **Facebook**, optimisé pour la documentation.
- Utilise des **composants React**.
- Basé sur Markdown mais permet des **éléments interactifs React**.
- 📖 [Documentation de Docusaurus](https://docusaurus.io/)

## 5. Pelican
- **Basé sur Python**, utile pour les blogs et les sites scientifiques.
- Supporte **reStructuredText et Markdown**.
- 📖 [Documentation de Pelican](https://docs.getpelican.com/)

## 6. Gatsby
- **Basé sur React**, hautement personnalisable.
- Peut être utilisé avec **Markdown, APIs, ou CMS**.
- 📖 [Documentation de Gatsby](https://www.gatsbyjs.com/)

## 7. Next.js (avec Exportation Statique)
- **Basé sur React**, idéal pour des pages hybrides statiques et rendues côté serveur.
- Nécessite une construction avant le déploiement.
- 📖 [Documentation de Next.js](https://nextjs.org/)

## Considérations de Déploiement
- **Jekyll** fonctionne directement avec GitHub Pages.
- **Hugo, MkDocs, Pelican, Gatsby, et Next.js** nécessitent une **étape de construction** avant le déploiement (par exemple, à l'aide de **GitHub Actions** ou d'un **pipeline CI/CD**).
- **Docusaurus** nécessite également une pré-construction.

Aimeriez-vous des recommandations en fonction de votre type de projet ? 🚀

<br>
<br>

-----
# Générateur de Site Statique Recommandé pour Votre Site de Recherche

Étant donné que vous êtes un **chercheur senior** et que vous avez besoin d'un site structuré avec un menu comprenant :
- **Accueil**
- **Publications**
- **Enseignement**
- **Logiciels**
- **Projets**
- **Popularisation**
- **Contact**

Je vous recommande **Jekyll** ou **MkDocs**, selon vos préférences :

## 🔹 Option 1 : Jekyll (Idéal pour des Sites Web Personnalisables)
- **Avantages** :
  - Intégré à **GitHub Pages** (pas de configuration supplémentaire nécessaire).
  - Supporte des thèmes (par exemple, [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/)).
  - Permet des mises en page personnalisées avec **Markdown + Liquid**.
  - Peut inclure un **support LaTeX** pour les contenus mathématiques.

- **Inconvénients** :
  - Nécessite un peu de configuration pour les thèmes avancés.
  - Les plugins nécessitent un processus de construction local.

📖 **Démarrer** : [Documentation de Jekyll](https://jekyllrb.com/)


## 🔹 Option 2 : MkDocs (Idéal pour Simplicité et Style de Documentation)
- **Avantages** :
  - Facile à configurer avec **Markdown**.
  - Idéal pour organiser des publications et projets de recherche.
  - Peut utiliser **Material for MkDocs**, qui est hautement personnalisable.
  - **Supporte nativement LaTeX** pour le contenu mathématique.

- **Inconvénients** :
  - Nécessite **GitHub Actions** pour le déploiement sur GitHub Pages.
  - Moins flexible pour des mises en page avancées comparé à Jekyll.

📖 **Démarrer** : [Documentation de MkDocs](https://www.mkdocs.org/)

---

## 🚀 Prochaines Étapes
Souhaitez-vous :
- Un **modèle pré-configuré** pour l'une de ces options ?
- Des conseils pour **personnaliser les thèmes** ?
- De l'aide pour configurer **GitHub Actions** pour le déploiement ?

Faites-le moi savoir, et je préparerai les fichiers nécessaires ! 🎯


<br>
<br>

-----


# Introduction à MkDocs

## Qu'est-ce que MkDocs ?

**MkDocs** est un **générateur de site statique** qui permet de créer des sites web en utilisant **Markdown**. Il est simple, rapide et idéal pour les sites de documentation, ce qui en fait un excellent choix pour les chercheurs.

## Fonctionnalités principales

- **Basé sur Markdown** : Écrivez du contenu dans des fichiers `.md`.
- **Rapide et léger** : Génère un site statique rapidement.
- **Support des thèmes** : Utilisez des thèmes comme [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).
- **Fonctionnalité de recherche** : Comprend une recherche en texte intégral.
- **Support de LaTeX** : Idéal pour les publications de recherche.

## Installation

MkDocs nécessite Python. Installez-le avec :

```bash
pip install mkdocs
```

Pour le **thème Material** (très recommandé) :

```bash
pip install mkdocs-material
```

## Créer un nouveau site

Exécutez les commandes suivantes :

```bash
mkdocs new mon-site
cd mon-site
```

Cela créera une structure de projet comme celle-ci :

```
mon-site/
│── docs/            # Les fichiers Markdown vont ici
│   ├── index.md     # Page d'accueil
│── mkdocs.yml       # Le fichier de configuration
```

## Structure d'un projet MkDocs

### 1. Le dossier `docs`

C'est ici que vous allez ajouter vos fichiers Markdown. Le fichier `index.md` est par défaut la page d'accueil de votre site.

### 2. Le fichier `mkdocs.yml`

Il contient la configuration du site, comme le titre, le thème, les plugins, et la structure du menu. Par exemple :

```yaml
site_name: Mon site de recherche
theme: material
nav:
  - Home: index.md
  - Publications: publications.md
  - Enseignement: enseignement.md
  - Projets: projets.md
  - Contact: contact.md
```

## Personnaliser le thème

Le thème **Material** est très populaire pour MkDocs. Il offre une personnalisation riche avec des fonctionnalités comme le **mode sombre**, des **animations** et la possibilité d'ajouter des **images et des vidéos**.

### Exemple de personnalisation dans `mkdocs.yml` :

```yaml
theme:
  name: material
  palette:
    primary: blue
    accent: light blue
  font:
    text: "Roboto"
    code: "Source Code Pro"
```

## Ajouter des plugins

MkDocs prend en charge plusieurs plugins pour étendre ses fonctionnalités. Par exemple, pour ajouter la **prise en charge de LaTeX** pour des équations mathématiques, vous pouvez ajouter le plugin `mkdocs-math` :

```bash
pip install mkdocs-math
```

Ensuite, dans `mkdocs.yml` :

```yaml
plugins:
  - mkdocs-math
```

## Générer le site

Une fois votre site configuré, vous pouvez le visualiser localement avec la commande suivante :

```bash
mkdocs serve
```

Cela démarrera un serveur local. Vous pourrez alors accéder à votre site à l'adresse `http://127.0.0.1:8000/`.

## Déployer sur GitLab Pages

Pour héberger votre site sur GitLab Pages, vous devez configurer GitLab CI/CD.

1. **Créer un fichier `.gitlab-ci.yml`** à la racine de votre projet avec le contenu suivant :

```yaml
image: python:3.8

before_script:
  - pip install mkdocs
  - pip install mkdocs-material

pages:
  script:
    - mkdocs build
  artifacts:
    paths:
      - public
  only:
    - main
```

2. **Pousser votre projet sur GitLab** : Quand vous poussez votre projet sur GitLab, GitLab Pages s'occupera de déployer automatiquement votre site.

Le site sera accessible via `https://<votre-nom-utilisateur>.gitlab.io/<nom-de-votre-projet>/`.

## Conclusion

MkDocs est un excellent outil pour les chercheurs qui souhaitent créer une documentation ou un site personnel en utilisant Markdown. Il est facile à configurer, très personnalisable et bien adapté à l’hébergement sur GitLab Pages.


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

<br>
<br>
---


Pour créer un site avec MkDocs en utilisant le thème **Material for MkDocs** et un menu spécifique, voici un exemple de configuration de base avec ton menu et une page supplémentaire pour "Dionaea". Tu pourras ensuite ajouter du contenu à chaque page et personnaliser les sections comme tu le souhaites.

### Étapes de base

1. **Installation de MkDocs et du thème Material** :
   - Si ce n’est pas encore fait, installe `mkdocs` et `mkdocs-material` :
     ```bash
     pip install mkdocs mkdocs-material
     ```

2. **Structure du dossier** :
   Organise ton projet MkDocs avec la structure suivante :
   ```
   my-website/
   ├── docs/
   │   ├── index.md
   │   ├── publications.md
   │   ├── teaching.md
   │   ├── software.md
   │   ├── projects.md
   │   ├── popularization.md
   │   ├── contact.md
   │   └── dionaea.md  # Page supplémentaire
   ├── mkdocs.yml
   ```

3. **Fichier `mkdocs.yml` (configuration)** :
   Voici un exemple de fichier de configuration pour `mkdocs.yml` avec ton menu et la page supplémentaire pour "Dionaea" :
   ```yaml
   site_name: "Mon Site de Recherche"
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
     - Dionaea: dionaea.md  # Page supplémentaire

   markdown_extensions:
     - toc:
         permalink: true
     - admonition
     - codehilite
     - pymdownx.arithmatex  # Pour le support LaTeX (si tu as besoin de formules)

   extra_css:
     - 'stylesheets/custom.css'  # Si tu veux ajouter un CSS personnalisé

   extra_javascript:
     - 'javascripts/custom.js'  # Si tu veux ajouter un JavaScript personnalisé
   ```

4. **Exemple de contenu pour une page (`index.md`)** :
   Voici un exemple de contenu pour la page d'accueil (`index.md`) :
   ```markdown
   # Bienvenue sur mon site de recherche

   Ce site présente mes travaux de recherche, mes publications, ainsi que mes projets et initiatives dans le domaine de la popularisation scientifique.

   ## À propos
   Je suis un chercheur en [sujet de recherche], et je suis passionné par [intérêts et projets].

   [Ajouter des liens vers les différentes sections ici]
   ```

5. **Page supplémentaire `dionaea.md`** :
   Si tu souhaites ajouter une page spécifique pour **Dionaea**, crée un fichier `dionaea.md` dans le dossier `docs/` et remplis-le avec le contenu que tu désires :
   ```markdown
   # Dionaea

   Dionaea est un projet [description du projet], qui a pour objectif de [but du projet].

   ## Détails
   [Explication détaillée du projet Dionaea et ses objectifs]
   ```

Avec cette configuration, tu aurais un site structuré avec un menu comprenant les sections principales : Home, Publications, Teaching, Software, Projects, Popularization, Contact, et une page supplémentaire pour **Dionaea**.

Tu peux maintenant compléter chaque fichier `.md` avec ton contenu spécifique et personnaliser davantage le style et les fonctionnalités du site.


<br>
<br>
----

Pour obtenir la liste des thèmes possibles dans MkDocs, tu peux procéder de plusieurs manières :

1. **Consulter la documentation officielle** :
   La liste des thèmes officiellement supportés dans MkDocs est disponible sur la [page des thèmes de MkDocs](https://pawamoy.github.io/mkdocs-gallery/themes/alabaster/) ou sur GitHub, où tu trouveras la documentation sur chaque thème ainsi que les étapes d'installation.

2. **Lister les thèmes installés avec MkDocs** :
   Si tu souhaites vérifier les thèmes installés dans ton environnement, tu peux exécuter cette commande :
   ```bash
   mkdocs --help
   ```
   Cela te donnera une liste d'options, et tu pourras repérer les thèmes qui peuvent être utilisés.

3. **Installer des thèmes supplémentaires** :
   Si tu veux installer d'autres thèmes, comme **Material for MkDocs**, tu peux le faire en exécutant la commande suivante :
   ```bash
   pip install mkdocs-material
   ```
   Une fois installé, tu pourras l'utiliser dans ton fichier `mkdocs.yml` en le configurant comme suit :
   ```yaml
   theme:
     name: "material"
   ```

Ainsi, tu auras la possibilité d'explorer et d'utiliser différents thèmes selon tes besoins.

Pas mauvais:

 - [cluster](https://kaliko.gitlab.io/mkdocs-cluster/)
 - [mkdocs](https://pawamoy.github.io/mkdocs-gallery/themes/mkdocs/)

<br>
<br>
----

If you prefer the menu to appear on the top banner instead of the left sidebar in MkDocs, you can customize the theme to achieve this layout. With the **Material for MkDocs** theme, it’s easy to change the navigation from a sidebar to a top navigation bar.

Here’s how you can modify your `mkdocs.yml` configuration to move the menu to the top:

### Steps to Move the Menu to the Top

1. **Ensure Material theme is installed** (if you haven’t already):
   ```bash
   pip install mkdocs-material
   ```

2. **Modify `mkdocs.yml` Configuration**:
   Update the configuration file (`mkdocs.yml`) to use the top navigation bar by setting the `nav` configuration and customizing the theme options:
   
   ```yaml
   site_name: "My Research Site"
   theme:
     name: "material"
     features:
       - navigation.tabs  # Enables top navigation bar

   nav:
     - Home: index.md
     - Publications: publications.md
     - Teaching: teaching.md
     - Software: software.md
     - Projects: projects.md
     - Popularization: popularization.md
     - Contact: contact.md
     - Dionaea: dionaea.md  # Additional page

   markdown_extensions:
     - toc:
         permalink: true
     - admonition
     - codehilite
     - pymdownx.arithmatex  # For LaTeX support if needed

   extra_css:
     - 'stylesheets/custom.css'  # Custom CSS if you want to tweak the layout

   extra_javascript:
     - 'javascripts/custom.js'  # Custom JavaScript if needed
   ```

### What This Configuration Does:
- **`navigation.tabs` feature**: This line tells the Material theme to display the navigation menu at the top of the page instead of in the sidebar.
- **`nav`**: This defines the sections of the site and how they appear in the menu.

### Additional Customization:
If you want to further tweak the appearance of the top navigation bar (like colors, size, etc.), you can add custom CSS to the `extra_css` section in the `mkdocs.yml`. For example, you can create a file `stylesheets/custom.css` with custom styles for the top menu.

With this setup, your site's navigation will appear on the top banner, making it more suitable for a clean and modern layout.


<br>
<br>
----

If you prefer to use the default **MkDocs** theme (instead of Material), and still want the menu to appear on the top banner rather than the left sidebar, you can achieve this with a simple configuration change. 

Here’s how you can modify your `mkdocs.yml` file to move the menu to the top while using the default **MkDocs** theme:

### Steps to Move the Menu to the Top with the MkDocs Theme

1. **Ensure MkDocs is installed** (if you haven’t already):
   ```bash
   pip install mkdocs
   ```

2. **Modify `mkdocs.yml` Configuration**:
   Update the configuration file (`mkdocs.yml`) to use the default MkDocs theme and enable the top navigation:

   ```yaml
   site_name: "My Research Site"
   theme:
     name: "mkdocs"  # Default MkDocs theme

   nav:
     - Home: index.md
     - Publications: publications.md
     - Teaching: teaching.md
     - Software: software.md
     - Projects: projects.md
     - Popularization: popularization.md
     - Contact: contact.md
     - Dionaea: dionaea.md  # Additional page

   markdown_extensions:
     - toc:
         permalink: true
     - admonition
     - codehilite
     - pymdownx.arithmatex  # For LaTeX support if needed

   extra_css:
     - 'stylesheets/custom.css'  # Custom CSS if you want to tweak the layout

   extra_javascript:
     - 'javascripts/custom.js'  # Custom JavaScript if needed
   ```

### What This Configuration Does:
- **`theme.name: "mkdocs"`**: This specifies that the default MkDocs theme is being used.
- **`nav`**: Defines the structure of the menu and its links.
- **Top Navigation**: The default MkDocs theme doesn't natively support a top navigation bar (it places the menu on the left). To move the menu to the top, additional customization is necessary via CSS.

### Customizing the Layout (Optional)
Since the MkDocs default theme places the navigation on the left by default, you can add custom CSS to modify the layout and position the menu at the top. Here’s how you can create a custom style:

1. Create a `stylesheets/custom.css` file.
2. Add the following CSS to move the sidebar to the top:

   ```css
   /* Custom CSS to move the navigation to the top */
   .md-sidebar {
     display: none;  /* Hide the left sidebar */
   }

   .md-nav {
     position: fixed;
     top: 0;
     width: 100%;
     background: #ffffff;  /* Change this to match your theme */
     box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
   }

   .md-main {
     margin-top: 60px;  /* Adjust content position to make space for the top nav */
   }
   ```

3. Link this CSS in your `mkdocs.yml`:

   ```yaml
   extra_css:
     - 'stylesheets/custom.css'  # Link to the custom CSS
   ```

With this setup, you will have a top navigation bar while still using the default MkDocs theme. The custom CSS hides the left sidebar and positions the navigation menu at the top of the page.

This allows you to use the simplicity of the MkDocs theme while customizing it to your preference.


<br>
<br>
----

Great! If you’re starting from a GitHub Pages repository (`fabien-campillo.github.io`) and currently have only a `README.md`, let’s walk through the steps to set up an MkDocs website from scratch.

### Step-by-Step Setup for MkDocs on GitHub Pages

1. **Set Up Your Local MkDocs Project**:
   First, you need to install MkDocs and create the basic structure for your website.

   - If you don’t have MkDocs installed, do it via:
     ```bash
     pip install mkdocs
     ```

   - Initialize the MkDocs project:
     ```bash
     mkdocs new my-website
     ```
     This will create a new folder `my-website/` with a sample project structure.

2. **Move Your GitHub Pages Repository to the MkDocs Project**:
   Since you already have a GitHub Pages repository (`fabien-campillo.github.io`), you need to move the content of `my-website/` into your GitHub Pages repository folder.

   - Clone your GitHub Pages repository to your local machine:
     ```bash
     git clone https://github.com/fabien-campillo/fabien-campillo.github.io
     cd fabien-campillo.github.io
     ```

   - Copy the contents of the `my-website/` directory (excluding `.git/`) into your repository folder. This will replace the current `README.md` file with the MkDocs project structure.

3. **Modify `mkdocs.yml`**:
   Edit the `mkdocs.yml` file to set up the site configuration and navigation. For example, here’s a basic configuration:

   ```yaml
   site_name: "Fabien Campillo - Research Website"
   theme:
     name: "mkdocs"  # Default MkDocs theme

   nav:
     - Home: index.md
     - Publications: publications.md
     - Teaching: teaching.md
     - Software: software.md
     - Projects: projects.md
     - Popularization: popularization.md
     - Contact: contact.md
     - Dionaea: dionaea.md  # Additional page

   markdown_extensions:
     - toc:
         permalink: true
     - admonition
     - codehilite
     - pymdownx.arithmatex  # For LaTeX support if needed

   extra_css:
     - 'stylesheets/custom.css'  # If you have custom CSS

   extra_javascript:
     - 'javascripts/custom.js'  # If you have custom JS
   ```

4. **Create Content Files**:
   Now, let’s add the content for your pages inside the `docs/` directory. Create `.md` files for each section you want to include:

   - **`index.

<br>
<br>
----

No, if you run `mkdocs new my-website`, it will create a new folder called `my-website` on your local machine with the necessary MkDocs files, but it won't be a live website at `https://my-website`.

Here’s the breakdown:
- **Local folder (`my-website`)**: This is where the MkDocs files are created on your computer. The folder will have the structure and content for your website, but it’s not yet published online.
  
- **GitHub Pages URL (`https://fabien-campillo.github.io`)**: This is the URL for your live website hosted on GitHub Pages. When you push the files from your local repository (e.g., `fabien-campillo.github.io`), GitHub will serve the site at `https://fabien-campillo.github.io`, not `https://my-website`.

To clarify, the name `my-website` is just the name of the directory created on your local machine. When you deploy it to GitHub Pages, the URL will follow the repository’s name on GitHub. In your case, it would be something like `https://fabien-campillo.github.io` (since that's the repository name). 

### If You Want to Host It on GitHub Pages:
If you're aiming to use GitHub Pages for your live website, follow these steps:

1. **Create a New Repository on GitHub** (if you haven’t already):
   - Go to GitHub and create a new repository named `fabien-campillo.github.io`.

2. **Clone the Repository Locally**:
   - Clone the repository to your local machine:
     ```bash
     git clone https://github.com/fabien-campillo/fabien-campillo.github.io
     cd fabien-campillo.github.io
     ```

3. **Initialize MkDocs in Your Repository**:
   - Now, you can initialize an MkDocs project in this folder:
     ```bash
     mkdocs new .
     ```
     This will create the necessary MkDocs files directly in your `fabien-campillo.github.io` directory (not in a subfolder like `my-website`).

4. **Add Your Content**:
   - You can now add your content to the `docs/` directory and configure your site in `mkdocs.yml`.

5. **Push to GitHub**:
   - Once you're ready, push your changes to GitHub:
     ```bash
     git add .
     git commit -m "Set up MkDocs website"
     git push origin main
     ```

6. **Set GitHub Pages Source**:
   - In the GitHub repository settings, configure GitHub Pages to use the `main` branch (or `master`) as the source and the root directory (`/`) for the site.

After this, your live site will be available at `https://fabien-campillo.github.io`!

### To Summarize:
- `mkdocs new my-website` creates a local folder, but the site won't be hosted at `https://my-website`.
- To host on GitHub Pages, push your MkDocs site to the repository `fabien-campillo.github.io`, and your live site will be at `https://fabien-campillo.github.io`.

<br>
<br>
----

