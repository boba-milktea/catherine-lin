# catherine-lin

> An interactive and dynamic portfolio website built using HTML and CSS
> animations, featuring a mobile-first design approach.

## Table of contents

- [catherine-lin](#catherine-lin)
  - [Table of contents](#table-of-contents)
  - [General info](#general-info)
  - [Screenshots](#screenshots)
  - [Technologies](#technologies)
  - [Setup](#setup)
  - [Code Examples](#code-examples)
  - [Features](#features)
  - [Status](#status)
  - [Inspiration](#inspiration)
  - [Contact](#contact)
  - [Instructions for use](#instructions-for-use)
  - [Code Quality Checks](#code-quality-checks)
  - [Continuous Integration (CI)](#continuous-integration-ci)
  - [Repo Setup](#repo-setup)

## General info

> This portfolio website is developed using HTML5 and augmented with CSS3 for
> scroll-triggered animations, ensuring dynamic content presentation. JavaScript
> is utilized to construct an interactive navigation bar. It's optimized for
> mobile devices using a mobile-first approach. Future iterations will focus on
> integrating a parallax scrolling effect

## Screenshots

![laptop screenshot 1](./planning/screenshot-1.png)

<hr />

![laptop screenshot 2](./planning/screenshot-2.png)

<hr />

![laptop screenshot 3](./planning/screenshot-3.png)

<hr />

<img src="./planning/screenshot-4.jpg" style="width: 400px" alt="mobile screenshot header" />
<hr />

<img src="./planning/screenshot-5.jpg" style="width: 400px" alt="mobile screenshot header" />
<hr />

<img src="./planning/screenshot-6.jpg" style="width: 400px" alt="mobile screenshot header" />

## Technologies

- Node 14.16.0
- VSC code
- JavaScript
- HTML
- CSS

## Setup

- `npm run start`
- `npm run install`

## Code Examples

```js
document.addEventListener("scroll", () => {
  const navBar = document.querySelector(".navbar");
  if (window.scrollY > 0) {
    navBar.classList.add("scrolled");
  } else {
    navBar.classList.remove("scrolled");
  }
});
```

```css
@supports (animation-timeline: view()) {
  .hero img {
    transform-origin: top;
    animation: hero-animation linear forwards;
    animation-timeline: view();
    animation-range: exit -200px;
  }
}
```

## Features

List of features ready and Todos for future development

- HTML5 and CSS
- CSS Scroll Animations
- JavaScript Navigation
- Mobile-First Design

To-do list:

- Parallax Scrolling Effect
- Accessibility Improvements
- Performance Optimization

## Status

Project is: _done_

## Inspiration

CSS animations by Keven Powell

## Contact

By [boba-milktea github](https://github.com/boba-milktea)

## Instructions for use

<details>
  <summary>Getting Started</summary>

<!-- a guide to using this repository -->

1. `git clone git@github.com:HackYourFutureBelgium/template-markdown.git`
2. `cd template-markdown`
3. `npm install`

## Code Quality Checks

- `npm run format`: Makes sure all the code in this repository is well-formatted
  (looks good).
- `npm run lint:ls`: Checks to make sure all folder and file names match the
  repository conventions.
- `npm run lint:md`: Will lint all of the Markdown files in this repository.
- `npm run lint:css`: Will lint all of the CSS files in this repository.
- `npm run validate:html`: Validates all HTML files in your project.
- `npm run spell-check`: Goes through all the files in this repository looking
  for words it doesn't recognize. Just because it says something is a mistake
  doesn't mean it is! It doesn't know every word in the world. You can add new
  correct words to the [./.cspell.json](./.cspell.json) file so they won't cause
  an error.
- `npm run accessibility -- ./path/to/file.html`: Runs an accessibility analysis
  on all HTML files in the given path and writes the report to
  `/accessibility_report`

## Continuous Integration (CI)

When you open a PR to `main`/`master` in your repository, GitHub will
automatically do a linting check on the code in this repository, you can see
this in the[./.github/workflows/lint.yml](./.github/workflows/lint.yml) file.

If the linting fails, you will not be able to merge the PR. You can double check
that your code will pass before pushing by running the code quality scripts
locally.

## Repo Setup

- Give each member **_write_** access to the repo (if it's a group project)
- Turn on GitHub Pages and put a link to your website in the repo's description
- Go to _General_ Section > check **Discussions**
- In the _Branches_ section of your repo's settings make sure the
  `master`/`main` branch must:
  - "_Require a pull request before merging_"
  - "_Require approvals_"
  - "_Dismiss stale pull request approvals when new commits are pushed_"
  - "_Require status checks to pass before merging_"
  - "_Require branches to be up to date before merging_"
  - "_Do not allow bypassing the above settings_"

</details>
