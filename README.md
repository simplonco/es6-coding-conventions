# es6-coding-conventions
ES2015, ES2017, eslint et coding conventions

## ES6, c'est quoi ?

C'est une nouvelle version de javascript qui va bientôt être utilisée sur tous les navigateurs

## ES6, pourquoi ?

* Ecrire moins de code
* Une version de javascript plus moderne

## Transpiler

* babel : https://babeljs.io/
* webpack avec babel-loader : https://github.com/babel/babel-loader
* create-react-app utilise webpack avec babel

## ES6 Katas et exercices :

* http://es6katas.org/
* corrections : (jusqu'à #45) : https://github.com/nullv01d/es6katas

* http://marijnhaverbeke.nl/talks/es6_falsyvalues2015

* https://babeljs.io/repl

* http://mycodekatas.github.io/javascript.html

## links :

* http://putaindecode.io/fr/articles/js/es2015/const-let-var/ [FR]
* http://putaindecode.io/fr/articles/js/es2015/template-strings/ [FR]
* http://putaindecode.io/fr/articles/js/es2015/object-literals/ [FR]
* http://putaindecode.io/fr/articles/js/es2015/classes/ [FR]
* http://putaindecode.io/fr/articles/js/es2015/arrow-functions/ [FR]
* http://putaindecode.io/fr/articles/js/es2015/defaults/ [FR]
* http://putaindecode.io/fr/articles/js/es2015/rest-spread/ [FR]
* http://putaindecode.io/fr/articles/js/es2015/array-methods-addition/ [FR]
* http://putaindecode.io/fr/articles/js/es2015/destructuring/ [FR]
* http://www.lilleweb.fr/js/2015/03/23/a-la-decouverte-de-es2015/ [FR]
* http://www.lilleweb.fr/js/2015/05/28/a-la-decouverte-es2015-partie-2/ [FR]
* http://www.lilleweb.fr/js/2015/06/20/a-la-decouverte-es2015-partie-3/ [FR]
* https://www.codeschool.com/courses/es2015-the-shape-of-javascript-to-come
* http://es6-features.org/
* https://babeljs.io/learn-es2015/
* https://kangax.github.io/compat-table/es6/
* http://es6katas.org/

* Bon article en français sur des sujets connexes :
  
  * https://tech.mozfr.org/tag/ES6%20en%20d%C3%A9tails
  * LES PROMISES : http://putaindecode.io/fr/articles/js/es2015/promises/ [FR]
  * notre stack front pour les prochain mois : http://putaindecode.io/fr/articles/frontend/2016-2-ans-avec-react-babel-webpack-et-cie/
  * les H.O.C en français : http://putaindecode.io/fr/articles/js/react/higher-order-component/)
  * Redux : http://putaindecode.io/fr/articles/js/redux/
  * Flow : http://putaindecode.io/fr/articles/js/flow/
  * Create-react-app (vous pouvez presque tout faire avec) : https://github.com/facebookincubator/create-react-app/blob/master/README.md
  * CI avec Travis : http://putaindecode.io/fr/articles/ci/travis-ci/
  * css-modules : http://putaindecode.io/fr/articles/css/modules/
  * Proxy ES6 : http://putaindecode.io/fr/articles/js/es2015/proxy/ (avec redux bien utilisé, on n'en a pas besoin)
  
 * en anglais :
 
  * https://babeljs.io/learn-es2015/
  * https://egghead.io/search?q=learn%20es6
  * https://github.com/lukehoban/es6features#readme
  * ES6 dans nodejs : https://codequs.com/p/Byvv408t/using-es6-import-export-in-node-js-babel-js/
  
 ## Exercice :
 
### Les variables en es6
 
* on utilise const et let à la place de var
* on utilise les Big Arrow function 
* on utilise des class pour declarer des objets
* on utilise des raccourcis
* on utilise des methodes pour les objets (nouvelle façon de  déclarer les methodes d'un objet)
* on utilise des noms de propriété calculé
* on utilise des promises
* on utilise des destructured
* on utilise des parametres par defaut
* on utilise des spread operators
* on utilise des generators

https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Op%C3%A9rateurs/Initialisateur_objet

https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Fonctions/D%C3%A9finition_de_m%C3%A9thode

https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Objets_globaux/Promise


### Les scopes et les scoped-blocks
 
#### Un scope en javascript est defini par function() { ... }.
 
 Toutes les variables utilisée à l'intérieur de la fonction utlisent ne sont accessible qu'à l'intérieur de la fonction
 
#### Un block en javascript est défini par { ... }. Par exemple :
* if() { ... } 
* for() { ... } 
* ()=>{ ... } 
* function(){ ... }
 
 En es5, les block n'ont pas de scope. Alors qu'en es6, les blocks ont un scope. Par exemple :
 
##### exemple 1

  ``` es5
 
 if(true) {
  var truc = 'bar'
 }
 
 console.log(truc):
 ``` 
 
 ``` es6

 if(true) {
  let truc = 'bar'
 }
 
  console.log(truc):
 ``` 
 
##### exemple 2

  ``` es5
 
 if(true) {
  var truc = 'bar'
 }
 
 console.log(truc):
 ``` 
 
 ``` es6

 if(true) {
  const truc = 'bar'
 }
 
  console.log(truc):
 ``` 
 
##### exemple 3

  ``` es5
 var truc = 'foo'
 
 if(true) {
  var truc = 'bar'
 }
 ``` 
 
 ``` es6
 let truc = 'foo'
 
 if(true) {
  let truc = 'bar'
 }
 ``` 
 
 ### Les big arrow functions
 
   ``` es5
 var truc = function() {
  
 }
 
 if(true) {
  var truc = 'bar'
 }
 ``` 
 
 ``` es6
 let truc = 'foo'
 
 if(true) {
  let truc = 'bar'
 }
 ``` 
 
 
 
 
 
 
 
 

