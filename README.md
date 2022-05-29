# Get Started

Prerequisites: 

- Node.js
- PostCSS VS Code extension

Run the local development environment.

*Build a project's package.json file:*

- `npm init -y`

*the -y flag means saying "yes" to all options.

*Build node_modules:*

- `npm i -D tailwindcss`

*Create a tailwind.config file:*

`npx tailwindcss init`

*In the `tailwind.config.js` file, add the following string to the content array:*

`content: ["./*.html"]`

*Create an `input.css` file in the root directory.*

*Then, add the following to the scripts key:*

`"scripts": {
    "build": "tailwindcss -i ./input.css -o ./css/style.css",
    "watch": "tailwindcss -i ./input.css -o ./css/style.css --watch"
  }`

After adding the scripts, run them in order in the terminal. The first script will build the tailwind output folder `css` and `style.css` file. The second script will rebuild and watch the files for any changes.

Now, create in `index.html` file in the root directory and link the output stylesheet. Then, add html to test if it is configured correctly.

