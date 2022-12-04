### from 2.6 to vue 3 with vue-compat (commit 2 & 3)

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

### from vue 3 with vue-compat to vue 3 (commit 4)
- run this command
```
npm r @vue/compat
```
delete vue.config.js (or take the one from vue3 default app)

### from vue cli to vite


### from vue-cli to vite (commit 5)

- run these commands
```
npm r @vue/cli-plugin-babel @vue/cli-plugin-eslint @vue/cli-plugin-typescript @vue/cli-plugin-unit-jest @vue/cli-service sass-loader
npm i -D vite
npm i -D vite-plugin-vue2 // for vue 2 projects
npm i -D @vitejs/plugin-vue // for vue 3 projects
npm i -D @vitejs/plugin-vue --force // for vue 2.7 projects
npm r core-js babel-eslint 
npm i eslint@8 eslint-plugin-vue@8
```
- delete babel.config.js 
- update .eslintrc.js
- create vite.config.js (not the same content if vue 2, vue 2.7, or vue 3)
- move index.html file and update it
- update package.json scripts 
