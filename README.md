# Svelte Snippets

Snippets for Svelte and Svelte-Kit (using TypeScript)

[VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=JakobKruse.svelte-kit-snippets)

## Snippets


### SVELTE KIT

<details>
<summary markdown="span"><b>sk</b>page -  Page (TypeScript)</summary>

```ts
<script lang="ts">
   import type { PageData } from './\$types';

   export let page: PageData;
   $1
</script>

$0
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>pagejs -  Page (JavaScript)</summary>

```ts
<script>
   /** @type {import('./\$types').PageData} */
   export let page;
   $1
</script>

$0
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>pl -  Page Load (TypeScript)</summary>

```ts
import type { PageLoad } from './\$types';

export const load: PageLoad = async (${1:event}) => {
   $2
   return {
     $0
   };
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>pljs -  Page Load (JavaScript)</summary>

```ts
/** @type {import('./\$types').PageLoad} */
export const load = async (${1:event}) => {
   $2
   return {
     $0
   };
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>psl -  Page Server Load (TypeScript)</summary>

```ts
import type { PageServerLoad } from './\$types';

export const load: PageServerLoad = async (${1:event}) => {
   $2
   return {
     $0
   };
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>psljs -  Page Server Load (JavaScript)</summary>

```ts
/** @type {import('./\$types').PageServerLoad} */
export const load = async (${1:event}) => {
   $2
   return {
     $0
   };
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>ll -  Layout Load (TypeScript)</summary>

```ts
import type { LayoutLoad } from './\$types';

export const load: LayoutLoad = async (${1:event}) => {
   $2
   return {
     $0
   };
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>ll -  Layout Load (JavaScript)</summary>

```ts
/** @type {import('./\$types').LayoutLoad} */
export const load = async (${1:event}) => {
   $2
   return {
     $0
   };
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>lsl -  Layout Server Load (TypeScript)</summary>

```ts
import type { LayoutServerLoad } from './\$types';

export const load: LayoutServerLoad = async (${1:event}) => {
   $2
   return {
     $0
   };
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>lsljs -  Layout Server Load (JavaScript)</summary>

```ts
/** @type {import('./\$types').LayoutServerLoad} */
export const load = async (${1:event}) => {
   $2
   return {
     $0
   };
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>a -  Page Actions (TypeScript)</summary>

```ts
import { Actions } from './\$types';

export const actions: Actions = {
   async ${1:default}({ $2 }) {
     $3
   }
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>ajs -  Page Actions (JavaScript)</summary>

```ts
/** @type {import('./\$types').Actions} */
export const actions = {
   async ${1:default}({ $1 }) {
     $2
   }
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>hh -  Hooks: Handle (TypeScript)</summary>

```ts
import type { Handle } from './\$types';

export const handle: Handle = async ({ request, resolve }) => {
   $1
   return resolve(request);
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>hhjs -  Hooks: Handle (JavaScript)</summary>

```ts
/** @type {import('./\$types').Handle} */
export const handle = async ({ event, resolve }) => {
   $1
   return resolve(event);
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>hf -  Hooks: HandleFetch (Typescript)</summary>

```ts
import type { HandleFetch } from './\$types';

export const handle: HandleFetch = async ({ request, fetch }) => {
   $1
   return resolve(request);
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>hfjs -  Hooks: HandleFetch (JavaScript)</summary>

```ts
/** @type {import('./\$types').HandleFetch} */
export const handle = async ({ request, fetch }) => {
   $1
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>he -  Hooks: Handle Error (TypeScript)</summary>

```ts
import type { HandleError } from './\$types';

export const handle: HandleError = async ({ error, event }) => {
   $2
};
```
</details>
    

<details>
<summary markdown="span"><b>sk</b>hejs -  Hooks: Handle Error (JavaScript)</summary>

```ts
/** @type {import('./\$types').HandleError} */
export const handle = async ({ error, event }) => {
   $1
};
```
</details>
    
    

### SVELTE

<details>
<summary markdown="span"><b>sv</b>comp -  Component (TypeScript)</summary>

```ts
<script lang="ts">
   $1
</script>

$0
```
</details>
    

<details>
<summary markdown="span"><b>sv</b>compjs -  Component (JavaScript)</summary>

```ts
<script>
   $1
</script>

$0
```
</details>
    

<details>
<summary markdown="span"><b>sv</b>disp -  Event Dispatcher</summary>

```ts
import { createEventDispatcher } from 'svelte';

const dispatch = createEventDispatcher<{ $1: $2}>()
$0
```
</details>
    

<details>
<summary markdown="span"><b>sv</b>dispjs -  Event Dispatcher (JavaScript)</summary>

```ts
import { createEventDispatcher } from 'svelte';

const dispatch = createEventDispatcher()
$0
```
</details>
    

<details>
<summary markdown="span"><b>sv</b>head -  Head Tag</summary>

```ts
<svelte:head>
   $1
</svelte:head>
$0
```
</details>
    

<details>
<summary markdown="span"><b>sv</b>fe -  For Each</summary>

```ts
{#each $1 as $2 ($3)}
   $0
{/each}
$0
```
</details>
    

<details>
<summary markdown="span"><b>sv</b>fee -  For Each else</summary>

```ts
{#each $1 as $2 ($3)}
   $4
{:else}
   $5
{/each}
$0
```
</details>
    

<details>
<summary markdown="span"><b>sv</b>if -  If</summary>

```ts
{#if $1}
   $2
{/if}
$0
```
</details>
    

<details>
<summary markdown="span"><b>sv</b>ife -  If Else</summary>

```ts
{#if $1}
   $2
{:else}
   $3
{/if}
$0
```
</details>
    

<details>
<summary markdown="span"><b>sv</b>ifei -  If Else If</summary>

```ts
{#if $1}
   $2
{:else if $3}
   $4
{/if}
$0
```
</details>
    

<details>
<summary markdown="span"><b>sv</b>await -  Await</summary>

```ts
{#await $1}
   $2
{:then $3}
   $4
{/await}
$0
```
</details>
    

<details>
<summary markdown="span"><b>sv</b>key -  Key</summary>

```ts
{#key $1}
   $2
{/key}
$0
```
</details>
    
    

## Note

The snippets include "$1", "$2"... which are placeholders for the cursor position. You can use the tab key to jump between them.

## License

MIT