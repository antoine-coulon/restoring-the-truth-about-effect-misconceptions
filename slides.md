---
# try also 'default' to start simple
theme: default
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://images.unsplash.com/photo-1471958680802-1345a694ba6d?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Antoine Coulon, Effect Paris # 1
  
  A la chasse aux idées reçues avec Effect

# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS (experimental)
css: unocss
---

## **A la chasse aux idées reçues avec Effect**

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
      <p class="mt-3">Créateur <b color="cyan">effect-introduction</b></p>
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

## **Le piège de la quête du savoir : les idées reçues**

Image

<!-- 

Comme n'importe quelle technologie qui émerge, beaucoup d'interrogations surviennent, surtout dans l'écosystème JS où les gens commencent à devenir perplexes avec des nouveaux frameworks, nouvelles libs à toutes les sauces.

Et comme toutes les nouvelles choses, des gens qui ne maîtrisent pas le sujet vont en parler, spéculer, sans avoir une profonde connaissance du sujet. Des idées reçues vont être avancées et des idées fausses vont aussi être conçues.

https://lapausephilo.fr/2016/02/18/je-sais-que-je-ne-sais-rien-socrate

D’après Socrate, la reconnaissance de notre ignorance est l’attitude nécessaire à adopter face à la quête du savoir.

Nos croyances et convictions façonnent notre perception du monde. Lorsqu’on est persuadé de savoir quelque chose, on abandonne une posture de recherche et on ne voit plus du monde que ce que l’on croit.
Toute certitude limite notre accès au savoir et renforce notre ignorance.

-->

---

## **Effect n'échappera pas à la règle**

- Technologie JavaScript (écosystème le plus mouvant)
- JavaScript fatigue

<!-- 
Comment combattre l'ignorance : la pédagogie autour des problèmes

-> Forcer les gens à prendre connaissance des problèmes

S'il y a bien quelque chose que j'ai appris pendant 2 ans d'Effect à accompagner des développeurs c'est de ne pas parler d'Effect, de parler
des problèmes, de JavaScript, de TypeScript, de la concurrence, DI, type-safety, Promises.

N'avancez pas Effect comme une solution révolutionnaire sans vous assurez que les problèmes sont d'abord compris.

-->

---

## **Le Pragmatisme au service du savoir**

<!-- 

Comment combattre l'ignorance : la pédagogie autour des problèmes

C'est d'ailleurs ce qui est définit dans le Pragmatisme, qui est à la base une école philosophique américaine fondée par Charles Sanders Peirce à la fin du 19e siècle. 
Le pragmatisme considère que n'est vrai que ce qui fonctionne en réalité.

Le pragmatisme met l'accent sur l'importance de tester et d'évaluer les idées par leur efficacité pratique. Avant de proposer une solution, il est crucial de comprendre pleinement les problèmes à résoudre et d'évaluer attentivement les conséquences possibles de toute action.

Donc être pragmatique c'est être penché sur les problèmes et apporter une solution qui fonctionne réellement, dans la vraie vie, dans les tranchées du software engineering :) 

-->

---

## **Détruisons les idées reçues à l'aide Pragmatisme**

Voyons ensemble certains idées reçues les plus répandues en ce qui concerne Effect

---

## Idée reçue n°1 : Effect, une niche pour les gurus FP

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

---

## Idée reçue n°2 : Un code très verbeux avec des fonctions étoiles ? wtf


---

## Idée reçue n°3 : Effect, uniquement requis pour des softwares très complexes


<!-- 
- Une boîte à outils _uniquement_ pour développer des software complexes
- Tout le monde fait face à X, on se confronte vite à la réalité, il n'y a pas de soft "simple"

Alors déjà il y a une idée reçue dans l'idée reçue.

Penser qu'il y a des soft très complexes et d'autres très faciles, c'est faux.
Alors oui certains sont plus simples que d'autres, mais en entreprise, combien sont réellement si faciles que ça ? Gérer des erreurs ? Gérer de la concurrence ? Gérer des ressources ? Maintenir du code, composer du code ?

-->

---

## Idée reçue n°4 : Effect tel un virus qui se répand dans toute la codebase

<!--

Alors celui là c'est un des mes préférés car il revient le plus souvent.

Les gens ont souvent peur qu'Effect soit une question d'all-in ou pas all-in.

- Effect peut être isolé à des endroits bien précis, convertis vers des Promises, Callbacks, code synchrone (si possible).

- Dire qu'Effect c'est un virus c'est comme parler de la contamination async/await (asynchrone se répand, la différence c'est que Effect fait l'abstraction entre sync/async)

-->

--- 

## Visez le savoir, fuyez l'ignorance

Toute certitude limite notre accès au savoir et renforce notre ignorance.


--- 

## Merci

