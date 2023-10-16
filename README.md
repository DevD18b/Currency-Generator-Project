# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

so am gonna talk about every single stuff on this project.
yaha pr khud keh hooks banate sikh rahe honge.
html css nahi sikh rahe honge.
hum yaha javascript likhna sikh rahe honge

actually ek currency builder project kya hota hai
jisme ek list of currency as an option aahh jaa rahi hogi apne pass set of amount gets converted to the from one currency to another.

ek hook toh apne aap meh ek method hai
jisme keh variable hota hai and function hota hai.
toh hook under the hood jab implement hua hoga toh uske creators neh bhi thoda
socha hoga kii ek variable hoga us pr hum operate kr rahe honge and then usko update krte jaayenge using setFunction.. right toh aisa toh hum bhi apna ek custom hooks create kr sakte hai lets see how.

first phase of the project is currency transformation keh liye data leh kr keh ana
us keh liye hum ek api use krte hai jo ki json formate meh data laati hai
but since that data is no where in the json woh actually ek string formate meh hota hai
toh hum usko purify krte hai json meh transform kr lete and useState hooks ka use kr keh store kara lete hai.

and finally we return data as it is.

now second phase is thoda ui create krna toh hum yeh ek ui bana kr usko reuse kr rahe honge
hum yaha pr jyada html css ki toh baat nhi karenge but we are gonna think
about the properties and parameter woh component ko form krne keh liye.
which can help working in the project
so usually hum ek component design kr lenge and usme kuch set of para meters daal denge.
jaise ki label --> from to.
onCurrencyChange
onAmountChange
selectCurrency.
amountDisabled
currrencyDisabled
etc toh yeh saare components will help us giving and charge jis seh ki hum UI meh change kr rahe honge.
and now finally yeh component ko hum call kr lenge humare main centeral point pr jisko hum kehte hai App.js
