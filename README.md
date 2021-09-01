

# VolarTypingThisRepro
Reproduction of an issue where 'this' inside a component is not typed.

## Steps to reproduce
install nx, 
```
npm install -g nx
```
install @nx-plus/vue with deps,
```
npm install @nx-plus/vue @nrwl/cypress --save-dev
```
Create a nx workspace and add a vue app
```
npx create-nx-workspace
nx g @nx-plus/vue:app frontend
```
Observe that the extended tsconfig in the app's folder contains `strict: true`, however, `this` inside a SFC is not typed.

----
or clone this repo and run

```
npm install
```
And look inside the `App.vue` component.
