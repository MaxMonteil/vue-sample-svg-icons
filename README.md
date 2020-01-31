# vue-sample-svg-icons

This is a fork of the project by Sarah Drasner which offers an opinionated example of how to use SVG icons in a Vue.js application.

[Original Repo](https://sdras.github.io/vue-sample-svg-icons/)

You can see more details about why it's set up this way in the [Vue Cookbook](https://vuejs.org/v2/cookbook/editable-svg-icons.html).

For this project I add more opinions and convert all icon related components into functional components.
The reason being that SVGs themselves are generally small files and normal components can add unnecessary overhead. This is ofcourse mostly apparent when you have a lot of icons.

You'll notice that this repo only changes the static SVGs and removes the animated ones because I don't own them and I didn't want to get into those just now.

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
