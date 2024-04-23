---
# try also 'default' to start simple
theme: default
# like them? see https://unsplash.com/collections/94734566/slidev
background: ./light.avif
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Antoine Coulon, Effect Paris #1
  
  À la chasse aux idées reçues avec Effect

# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS (experimental)
css: unocss
---

## **À la chasse aux idées reçues avec Effect**

<br>

<h4 class="mt-10">
  Antoine Coulon @ Effect Paris #1
</h4>

---

<div class="grid grid-cols-10 gap-x-4 pt-5 pr-10 pl-10">

<div class="col-start-1 col-span-7 grid grid-cols-[3fr,2fr] mr-10">
  <div class="pb-4">
    <h1><b>Antoine Coulon</b></h1>
    <div class="leading-8 mt-8 flex flex-col">
      <p class="mt-3">Lead Software Engineer @ <b color="cyan">evryg</b></p>
      <p class="mt-3">Créateur <b color="cyan">skott</b></p>
      <p class="mt-3">Auteur <b color="cyan">effect-introduction</b></p>
      <p class="mt-3">Contributeur <b color="cyan">Rush.js, NodeSecure</b></p>
    </div>
  </div>
  <div class="border-l border-gray-400 border-opacity-25 !all:leading-12 !all:list-none my-auto">
  </div>

</div>

<div class="pl-20 col-start-8 col-span-10">
  <img src="https://avatars.githubusercontent.com/u/43391199?s=400&u=b394996dd7ddc0bf7a317185ee9c378d5b609e12&v=4" class="rounded-full w-40 margin-0-auto" />

  <div class="mt-5">
    <div class="mb-4 flex justify-between"><ri-github-line color="blue"/> <b color="opacity-30 ml-2">antoine-coulon</b></div>
    <div class="mb-4 flex justify-between"><ri-twitter-line color="blue"/> <b color="opacity-30 ml-2">c9antoine</b></div>
    <div class="mb-4 flex justify-between"><ri-user-3-line color="blue"/> <b color="opacity-30 ml-2">dev.to/antoinecoulon</b></div>
  </div>
</div>

</div>

<style>
  h1 {
    color: #4c7fff;
  }
  img {
    margin: 0 auto;
  }
</style>

---
layout: image-right
image: socrate.jpeg
---

## <b>Le piège de la quête du savoir : l'idée reçue</b>

<div class="mt-10">
  <ul>
    <li>Se transmet rapidement à cause de la persuasion individuelle ou collective</li>
    <li>L'idée reçue est un frein à l'apprentissage et renforce l'ignorance</li>
  </ul>
</div>

<div v-click class="mt-15">

<h3 class="ml-5"><i>"Tout ce que je sais, c'est que je ne sais rien."</i></h3>

<div class="flex justify-end mr-20">
  <h3 class="mt-3">- Socrate</h3>
</div>

</div>

<!-- 

Comme n'importe quelle technologie qui émerge, beaucoup d'interrogations surviennent, surtout dans l'écosystème JS où les gens commencent à devenir perplexes avec des nouveaux frameworks, nouvelles libs à toutes les sauces.

Et comme toutes les nouvelles choses, des gens qui ne maîtrisent pas le sujet vont en parler, spéculer, sans avoir une profonde connaissance du sujet. Des idées reçues vont être avancées et des idées fausses vont aussi être conçues.

https://lapausephilo.fr/2016/02/18/je-sais-que-je-ne-sais-rien-socrate

D’après Socrate, la reconnaissance de notre ignorance est l’attitude nécessaire à adopter face à la quête du savoir.

Nos croyances et convictions façonnent notre perception du monde. Lorsqu’on est persuadé de savoir quelque chose, on abandonne une posture de recherche et on ne voit plus du monde que ce que l’on croit.
Toute certitude limite notre accès au savoir et renforce notre ignorance.

Incompétence consciente -> quatres étapes de l'apprentisage

-->
<style>
  h2 {
    color: #4c7fff;
  }
</style>

---

## **Les quatre étapes de la compétence**

<div class="flex justify-center mt-9">
  <img src="/competence.jpg" width="600" />
</div>

<style>
  h2 {
    color: #4c7fff;
  }
</style>
---


## **Effect ne pouvait pas échapper à la règle...**


<div class="flex mt-15 justify-around">

<div>
  <br><b color="orange">|></b> librairie TypeScript
  <br><b color="orange">|></b> programmation fonctionnelle 
  <br><b color="orange">|></b> effects
  <br><b color="orange">|></b> runtime
  <br><b color="orange">|></b> dependency injection, testing
  <br><b color="orange">|></b> flatMap, generators, pipeable APIs
</div>

  <img src="/bored.gif" width="400" />
</div>

<!-- 
Comment combattre l'ignorance : la pédagogie autour des problèmes

-> Forcer les gens à prendre connaissance des problèmes

S'il y a bien quelque chose que j'ai appris pendant 2 ans d'Effect à accompagner des développeurs c'est de ne pas parler d'Effect, de parler
des problèmes, de JavaScript, de TypeScript, de la concurrence, DI, type-safety, Promises.

N'avancez pas Effect comme une solution révolutionnaire sans vous assurez que les problèmes sont d'abord compris.

-->

<style>
  h2 {
    color: #4c7fff;
  }
</style>

---
layout: image-right
image: pragmatism.jpeg
---

## **Le Pragmatisme au service du savoir**

École philosophique américaine fondée par Charles Sanders Peirce à la fin du XIXe siècle.

- Comprendre les problèmes avant d'acter des solutions  

- Tester et évaluer les idées par leur efficacité pratique

- La vérité n'existe pas <i>a priori</i> mais se révèle par l'expérience

<!-- 

Comment combattre l'ignorance : la pédagogie autour des problèmes

C'est d'ailleurs ce qui est définit dans le Pragmatisme, qui est à la base une école philosophique américaine fondée par Charles Sanders Peirce à la fin du 19e siècle. 
Le pragmatisme considère que n'est vrai que ce qui fonctionne en réalité.

Le pragmatisme met l'accent sur l'importance de tester et d'évaluer les idées par leur efficacité pratique. Avant de proposer une solution, il est crucial de comprendre pleinement les problèmes à résoudre et d'évaluer attentivement les conséquences possibles de toute action.

Donc être pragmatique c'est être penché sur les problèmes et apporter une solution qui fonctionne réellement, dans la vraie vie, dans les tranchées du software engineering :) 

-->

<style>
  h2 {
    color: #4c7fff;
  }
</style>
---

## **Détruisons les idées reçues à l'aide du Pragmatisme**

Construisons donc <b color="green">la réalité et la vérité</b> autour d'Effect à partir de <b color="green">l'expérience</b> et non pas des <b color="orange">a priori</b>

<div class="flex justify-center mt-9">
  <img src="/no-way.gif" />
</div>

<style>
  h2 {
    color: #4c7fff;
  }
</style>

---

## **Idée reçue n°1 : <b color="orange">"Effect est une niche pour les gourous FP"</b>**

<div class="flex mt-5">

<div class="mt-15">

<h3 class="ml-5"><i>"Forget that there is even a thing called Functional Programming"</i></h3>


<div class="flex justify-end mr-20">
  <h3 class="mt-3">- Effect website</h3>
</div>

<div v-click class="mt-15">
  <h3>Vérité : <b color="green">Effect s'adresse aux développeurs qui ciblent des apps robustes, maintenables et de qualité.</b> </h3>
</div>

</div>

<div>
  <img src="/monad.webp" />
</div>

</div>


<!-- 
Effect est une niche pour les gurus FP qui font des side-projects avec Haskell ou OCaml sur leur temps libre

Des personnes utilisent Haskell/OCaml ? Mince c'est donc vrai alors...

- Une niche pour les devs FP
  - fait l'abstraction de concepts FP, veut s'éloigner du jargon. Parler de ZIO et des problématiques auxquelles ils ont fait face et comment ils se sont séparés du jargon

Effect a attiré les gens qui viennent du FP en premier car ce sont des personnes qui avaient déjà compris bcp de choses que FP résoud.

Pour autant, Effect ne s'adresse pas uniquement aux FPers...

D'ailleurs syntaxe impérative vs pipeable API

ça permet jsutement la transition vers les générateurs
-->

<style>
  h2 {
    color: #4c7fff;
  }
</style>


---

## **Idée reçue n°2 : <b color="orange">"Effect est uniquement utile pour des apps complexes"</b>**

<div class="flex justify-center mt-3 mb-5">
  <img src="/complexity.png" width="700" />
</div>

<div v-click>
  <h3>Vérité : <b color="green">Effect réduit la complexité des applications.</b></h3>
</div>


<!-- 
- Une boîte à outils _uniquement_ pour développer des software complexes
- Tout le monde fait face à X, on se confronte vite à la réalité, il n'y a pas de soft "simple"

Alors déjà il y a une idée reçue dans l'idée reçue.

Penser qu'il y a des soft très complexes et d'autres très faciles, c'est faux.
Alors oui certains sont plus simples que d'autres, mais en entreprise, combien sont réellement si faciles que ça ? Gérer des erreurs ? Gérer de la concurrence ? Gérer des ressources ? Maintenir du code, composer du code ?

-->

<style>
  h2 {
    color: #4c7fff;
  }
</style>


---

## **Idée reçue n°3 : <b color="orange">"Effect est un virus qui contamine toute la codebase"</b>**

<div class="mt-10 mb-5">
<ul>
<li> Possibilité d'utiliser Effect de manière purement localisée : <u>runPromise | runCallback | runSync</u> </li>

<li> Ce qui contamine réellement une codebase : gestion de l'asynchrone vs du synchrone  </li>
</ul>

<div class="flex justify-around mt-5 mb-3">

  <div v-click>
    <u>Async vs Sync</u>
    <ul>
      <li>
        Gestion des erreurs : <b color="orange">différente</b> 
      </li>
      <li>
        Control flow : <b color="orange">différent</b>
      </li>
      <li>
        Typings : <b color="orange">différent</b>
      </li>
      <li>
        Primitives : <b color="orange"> différentes </b> (Callbacks, Promises, etc.)
      </li>
      <li>
        Syntaxe : <b color="orange"> différente </b>
      </li>
    </ul>
  </div>

  <div v-click>
    <u>Effect</u>
    <ul>
      <li>
        Gestion des erreurs : <b color="green">pareil</b> 
      </li>
      <li>
        Control flow : <b color="green">pareil</b>
      </li>
      <li>
        Typings : <b color="green">pareil</b>
      </li>
      <li>
        Primitives : <b color="green"> pareil </b> (Effect)
      </li>
      <li>
        Syntaxe : <b color="green"> pareil </b>
      </li>
    </ul>
  </div>

  <div>



  </div>

</div>

</div>  

<div v-click>
  <h3>Vérité : <b color="green">Effect est plus un antidote qu'un virus.</b></h3>
</div>

<!--

Alors celui là c'est un des mes préférés car il revient le plus souvent.

Les gens ont souvent peur qu'Effect soit une question d'all-in ou pas all-in.

- Effect peut être isolé à des endroits bien précis, convertis vers des Promises, Callbacks, code synchrone (si possible).

- Dire qu'Effect c'est un virus c'est comme parler de la contamination async/await (asynchrone se répand, la différence c'est que Effect fait l'abstraction entre sync/async

-->

<style>
  h2 {
    color: #4c7fff;
  }
</style>

--- 

## **À la conquête du savoir**

<div class="mt-10">
  <ul>
    <li>S'assurer que les problèmes taclés par la solution sont bien <u>maîtrisés</u></li>
    <li>Valoriser l'<u>humilité intellectuelle</u> : quatre étapes de la compétence en tête </li>
    <li>S'appuyer sur la <u>pratique</u>, l'<u>expérience</u> et des cas concrets pour établir la vérité</li>
  </ul>
</div>

<div class="mt-10" v-click>
<i v-click>"Toute certitude limite notre accès au savoir et renforce notre ignorance. Savoir que l'on est ignorant est le meilleur moyen de ne plus en être un...</i>
</div>

<br>

<div>
<i v-click>...et surtout n'oubliez pas de npm install effect"</i>
</div>

<br>

<div v-click class="text-center mr-20"><b>- Socrate</b></div>

<style>
  h2 {
    color: #4c7fff;
  }
</style>


--- 

## **Merci**

Lien des slides: https://antoine-coulon.github.io/restoring-the-truth-about-effect-misconceptions

- L'affirmation Socratique : https://www.cairn.info/revue-l-enseignement-philosophique-2010-4-page-38.htm
- Quatre étapes de la compétence : https://fr.wikipedia.org/wiki/Les_quatre_%C3%A9tapes_de_la_comp%C3%A9tence
- Le Pragmatisme : https://fr.wikipedia.org/wiki/Pragmatisme
- Effect : https://effect.website

<style>
  h2 {
    color: #4c7fff;
}
</style>
