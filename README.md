# Gulp HTML BoilerTemplate

A front-end development BoilerTemplate to accelerate your workflow and assist in converting Figma designs to HTML/CSS using a modular approach or blocks. It already includes the Bootstrap v5 at initial.

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
  - [Project Structure](#project-structure)
  - [Development Workflow](#development-workflow)
  - [Building for Production](#building-for-production)
- [Contributions](#contributions)
- [License](#license)

## Features

- Modular development structure for improved maintainability.
- Gulp tasks for automating common front-end development tasks.
- Easily convert Figma designs to HTML/CSS.
- Streamlined development workflow.
- AutoPrefixes are used for browser compatibility.
- Image optimization.
- Fonts are preloaded.

## Getting Started

### Prerequisites

Before you begin, ensure you have met the following requirements:

- [Node.js](https://nodejs.org/) and npm (Node Package Manager) installed on your system.

### Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/saadtanvir1994/gulp-html-boilertemplate.git
   ```

2. Navigate to the project directory:
    ```bash
   cd gulp-html-boilertemplate
   ```

3. Install the project dependencies:
    ```bash
   npm install
   ```
4. Run the development server
   ```bash
   npm run dev
   ```

## Usage

### Project Structure
The project is structured as follows:
  ```
├── src/
│ ├── index.html
| ├── fonts/
│ ├── img/
│ ├── js/
│ │ ├── vendors/
│ │ ├── app.js
│ ├── partials/
│ ├── sass/
│ │ ├── vendors/
│ │ ├── app.css
├── gulpfile.js
├── package.json
├── package-lock.json
  ```
`partials` contains blocks. Which you can import on different pages.
`vendors` folders are used to import third-party libraries like Bootstrap, swiper slider, etc. and they would come up as one file with names `vendors.min.css` and `vendors.min.js` in `production`. You need to number them so they can concat in the `production`. You can create more pages like about.html in `src`
### Development Workflow
You need to re-run the development server once the files are added to the vendor folder or you can add a watch to it using the `gulpfile.js`
### Building for Production
You need to run `npm run build` to create a `build` folder that you can deliver to your client.

## Contributions
Contributions are welcome! If you have suggestions, improvements, or bug fixes, please create a pull request. For major changes, please open an issue first to discuss the proposed changes.

## License
This project is licensed under the **MIT License**.
