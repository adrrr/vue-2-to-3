### from 2.6 to 2.7

- run these commands
```
vue upgrade //to check vue-cli is the latest
npm r vue //removes vue2
npm r vue-template-compiler //not needed for vue3
npm i vue //installs vue3
npm i @vue/compat
npm i -D @vue/compiler-sfc
npm i @vue/test-utils@2
npm install @vue/vue3-jest@27
```
<sub>where 27 is the version of jest</sub>
- replace "export default Vue.extend({" with "export default {"
- update vue.config.js
- update shim-vue.d.ts (for unit tests)

### from vue-cli to vite

- run these commands
```
npm r @vue/cli-plugin-babel @vue/cli-plugin-eslint @vue/cli-plugin-typescript @vue/cli-plugin-unit-jest @vue/cli-service sass-loader
npm i -D vite
npm i -D vite-plugin-vue2 // for vue 2 project3
npm i -D @vitejs/plugin-vue // for vue 3 project3
npm i -D @vitejs/plugin-vue --force // for vue 2.7 project
npm r core-js babel-eslint 
npm i estlint@8 eslint-plugin-vue@8
```
- delete babel.config.js 
- update .eslintrc.js
- create vite.config.js (not the same content if vue 2, vue 2.7, or vue 3)
- move index.html file and update it
- update package.json scripts 