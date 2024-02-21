---
# try also 'default' to start simple
theme: default
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://images.unsplash.com/photo-1471958680802-1345a694ba6d?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
monaco: true
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Antoine Coulon, Effect Days # 1
  
  Building skott: a journey of Effect-Driven Development
# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS (experimental)
css: unocss
---

## **Building skott: a journey of Effect-Driven Development**

<br>

<h4 class="mt-10">
  Antoine Coulon @ Effect Days #1
</h4>

---

<div class="grid grid-cols-10 gap-x-4 pt-5 pr-10 pl-10">

<div class="col-start-1 col-span-7 grid grid-cols-[3fr,2fr] mr-10">
  <div class="pb-4">
    <h1><b>Antoine Coulon</b></h1>
    <div class="leading-8 mt-8 flex flex-col">
      <p class="mt-3">Lead Software Engineer @ <b color="cyan">evryg</b></p>
      <p class="mt-3">Author of <b color="cyan">skott</b></p>
      <p class="mt-3">Author of <b color="cyan">effect-introduction</b></p>
      <p class="mt-3">Contributing to <b color="cyan">Rush.js, NodeSecure</b></p>
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

## **The problem: graphs are everywhere, but hidden**

<div class="mt-15">
  <h3><strong>What is missing?</strong></h3>
  <h3 class="mt-5">- APIs to use graphs or build tools on top</h3>
  <h3 class="mt-5">- Revealing circular/implicit/hidden/unused dependencies</h3>
  <h3 class="mt-5">- Offering architecture/design analysis capabilities</h3>
  <h3 class="mt-5">- Exposing general purpose information, metadata, third-party dependencies...</h3>
</div>

<style>
  h2 {
    color: #4c7fff;
  }
</style>

---
layout: image-right
image: skott-graph.png
---

## **skott does all of that**


<div class="mt-15">
  <h4 class="mt-5">- Supports <strong>JavaScript</strong> + <strong>TypeScript</strong> projects</h4>
  <h4 class="mt-5">- Can be used via <strong>CLI</strong> or <strong>JavaScript API</strong></h4>
  <h4 class="mt-5">- Written with <strong>TypeScript</strong>, running on <strong>Node.js</strong></h4>
  <h4 class="mt-5">- Focused on providing great <strong>developer experience</strong></h4>
  <h4 class="mt-5">- Lot of <strong>display modes</strong> out of the box</h4>
</div> 

<style>
  h2 {
    color: #4c7fff;
  }
</style>

---

## **skott needs what all softwares needs**

<div class="grid grid-cols-2 gap-x-4 pt-5">

<div v-click>
  <h3><strong>Mostly I/O</strong></h3>
  <ul> 
    <li>reading the whole file tree</li> 
    <li>module resolution</li>
    <li>write/read operations with local cache </li> 
  </ul>

<!-- 
  ```ts
  for await (const rootFile of this.fileReader.readdir(
      this.fileReader.getCurrentWorkingDir(),
      this.config.fileExtensions
    )) {
      const rootFileContent = await this.fileReader.read(rootFile);

      // [...]

      if (this.config.incremental) {
        this.#cacheHandler.addSourceFile(rootFile, rootFileContent);
      }

      await this.addNode(rootFile);
      await this.collectModuleDeclarations(rootFile, rootFileContent);
    }
  ``` -->

  <img src="/code.png" class="mt-3" />

</div>

<div v-click>
  <h3><strong>Also common things</strong></h3>  
  logging, control flows, error recovery, dependency injection, concurrency...

  <img src="/code-2.png" class="mt-3" />

</div>
</div>

<style>
  h2 {
    color: #4c7fff;
  }
</style>

---

## **Developing reliable software is hard**

<strong>When it comes to developing software, we can put in practice various disciplines</strong>

<div class="grid grid-cols-2 gap-x-4 pt-5">

<div v-click>
  <b>Test-Driven Development (TDD)</b>

  <img width="500" src="/test-pass.gif" class="mt-5" />
</div>

<div v-click>
  <b>Type-Driven Development (TDD as well)</b>

  <img width="500" src="/type-level.gif" class="mt-5" />
</div>

</div>

<style>
  h2 {
    color: #4c7fff;
  }
</style>

---

## **Introducing Effect-Driven Development**


<div class="mt-10">
  <h3><strong>A streamlined and unified way of developing software</strong></h3>
  <h3 class="mt-5">Effect enables both <strong>Test</strong> and <strong>Type-Driven Development</strong></h3>
  <h4 class="mt-5">- <strong>Dependency Inversion Principle</strong> at heart</h4>
  <h4 class="mt-5">- Extreme <strong>type-safety</strong></h4>
  <h4 class="mt-5">- Fast <strong>feedback loop</strong> overall</h4>
</div>

<div class="mt-5 flex justify-center">
  <img src="/effect.png" class="rounded-full w-40 margin-0-auto" />
</div>

<style>
  h2 {
    color: #4c7fff;
  }
</style>

---

## **The trap: Third-Party-Driven Development**

<div class="mt-15">
  <h3 class="mt-5">🧱 &nbsp; Composition between all dependencies is hard</h3>
  <h3 class="mt-5">⏳ &nbsp; Maintenance cost</h3>
  <h3 class="mt-5">📈 &nbsp; Learning curve</h3>
  <h3 class="mt-5">🔌 &nbsp; Compatibilities issues</h3>
  <h3 class="mt-5">⚠️ &nbsp; Higher vulnerability surface</h3>
</div>

<style>
  h2 {
    color: #4c7fff;
  }
</style>

---

## **Select your difficulty level: Either<HardMode, EasyMode>**

Two Options, or one Either...

<div class="grid grid-cols-2 gap-x-4 pt-5">

<div v-click>
  Option[HardMode]: <strong>npm install *universe*</strong>

   😵‍💫 A fragmented ecosystem complexifying composability and maintenability
</div>

<div v-click>
  Option[EasyMode]: <strong>npm install effect</strong>

  🫵 A streamlined way of developing software with unified standard library and ecosystem

</div>
</div>

<div v-click>
```json {monaco-diff}
{
  "fp-ts": "*",
  "async": "*",
  "p-queue": "*",
  "p-retry": "*",
  "inversify": "*",
  "ts-pattern": "*",
  "ts-results": "*",    
  "neverthrow": "*",
  "ramda": "*",
  "winston": "*"
}
~~~
{
  "effect": "latest"
}
```
</div>

<style>
  h2 {
    color: #4c7fff;
  }
</style>

--- 
layout: image
---

## **Spoiler: I chose life on easy mode for skott**

<br>

```ts
import { Either } from "effect";

declare const lifeChoice: Either.Either<HardMode, EasyMode>;
const easyModeOnly = lifeChoice.pipe(Effect.orDie, Effect.runSync);
```


<div class="flex mt-5 ml-15 mr-15 justify-center">
  <img src="/migrate-effect.png" width="600">
</div>



<style>
  h2 {
    color: #4c7fff;
  }
</style>
---

## **Thanks for listening**

<div class="grid grid-cols-10 gap-x-4 pt-5 pr-10 pl-10">

<div class="col-start-1 col-span-8 grid grid-cols-[3fr,2fr] mr-10">
  <div class="pb-4">
    <ul class="leading-8 mt-8 flex flex-col">
    <li><b>skott</b>: <b color="cyan">https://github.com/antoine-coulon/skott</b> </li>
    <li><b>Effect introduction</b>: <b color="cyan">https://github.com/antoine-coulon/effect-introduction</b></li>
    </ul>
  </div>

  ### **Questions?**
</div>

<div class="pl-20 col-start-9 col-span-10">
  <img src="/cyclops.jpg" class="rounded-full w-40 margin-0-auto" />
  <img src="/effect.png" class="rounded-full w-40 margin-0-auto mt-4" />
</div>

</div>

<style>
  h2 {
    color: #4c7fff;
  }
</style>