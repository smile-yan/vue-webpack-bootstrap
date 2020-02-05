# vue-webpack-bootstrap

A demo to create one project with vue, webpack and bootstrap without using jQuery.

## Build Setup

``` bash
# clone 
git clone https://github.com/smile-yan/vue-webpack-bootstrap.git
cd vue-webpack-bootstrap

# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report

# run unit tests
npm run unit

# run e2e tests
npm run e2e

# run all tests
npm test
```

## How to create 
First of all, make sure that you have installed node.js(version>=8.0).

```bash
# install vue-cli  
cnpm install vue-cli -g

# init webpack project
vue init webpack my-project

# enter the project created and install bootstrap4 and bootstrapVue
cd my-project
cnpm install bootstrap-vue --save
cnpm install bootstrap --save
```

Then you should edit `src/router/index.js` or `src/router/app.js` to configure for bootstrap.
Add some words as follows:

```javascript
import { BootstrapVue, IconsPlugin } from 'bootstrap-vue'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'

// Install BootstrapVue
Vue.use(BootstrapVue)
// Optionally install the BootstrapVue icon components plugin
Vue.use(IconsPlugin)
```

Finally you should edit the App.vue to test 
Add some words as follows:
```html
<b-card
      header="featured"
      header-tag="header"
      footer="Card Footer"
      footer-tag="footer"
      title="Title"
    >
      <b-card-text>Header and footers using props.</b-card-text>
      <b-button href="#" variant="primary">Go somewhere</b-button>
    </b-card>
```

Then you could input `npm run dev` and visit http://localhost:8080.

Thanks.

> Smileyan
> 2020.2.5 