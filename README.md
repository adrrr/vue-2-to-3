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
