# Svelte Snippets

Snippets for Svelte and Svelte-Kit (using TypeScript)

## Snippets


### SVELTE KIT

<details>
<summary markdown="span">skl - SvelteKit Page Server Load</summary>

```ts
export const load = async ({ $1 }) => {
   $2
   return {
     $3
   };
};
```
</details>
    

<details>
<summary markdown="span">skpl - SvelteKit Page Server Load with explicit typing for PageLoad</summary>

```ts
export const load: PageLoad = async ({ $1 }) => {
   $2
   return {
     $3
   };
};
```
</details>
    

<details>
<summary markdown="span">skpsl - SvelteKit Page Server Load with explicit typing for PageServerLoad</summary>

```ts
export const load: PageServerLoad = async ({ $1 }) => {
   $2
   return {
     $3
   };
};
```
</details>
    

<details>
<summary markdown="span">skll - SvelteKit Page Server Load with explicit typing for LayoutServerLoad and context</summary>

```ts
export const load: LayoutServerLoad<{ $1 }> = async ({ $2 }) => {
   $3
   return {
     $4
   };
};
```
</details>
    

<details>
<summary markdown="span">sklsl - SvelteKit Page Server Load with explicit typing for LayoutServerLoad and context</summary>

```ts
export const load: LayoutServerLoad<{ $1 }> = async ({ $2 }) => {
   $3
   return {
     $4
   };
};
```
</details>
    

<details>
<summary markdown="span">ska - SvelteKit Page Actions</summary>

```ts
export const actions = {
   async ${1:default}({ $2 }) {
     $3
     return {
       $4
     };
   }
};
```
</details>
    

<details>
<summary markdown="span">skat - SvelteKit Page Actions with explicit typing</summary>

```ts
export const actions: Actions = {
   async ${1:default}({ $2 }) {
     $3
     return {
       $4
     };
   }
};
```
</details>
    
    

### SVELTE

<details>
<summary markdown="span">svts - Svelte Typescript script tag</summary>

```ts
<script lang="ts">
$0
</script>
```
</details>
    

<details>
<summary markdown="span">svdisp - Svelte event dispatcher</summary>

```ts
const dispatch = createEventDispatcher()
$0
```
</details>
    

<details>
<summary markdown="span">svdispt - Svelte event dispatcher with type annotations</summary>

```ts
const dispatch = createEventDispatcher<{ $1: $2}>()
$0
```
</details>
    

<details>
<summary markdown="span">svhead - Svelte head tag</summary>

```ts
<svelte:head>
   $1
</svelte:head>
$0
```
</details>
    

<details>
<summary markdown="span">svfe - Svelte for each</summary>

```ts
{#each $1 as $2 ($3)}
   $0
{/each}
$0
```
</details>
    

<details>
<summary markdown="span">svfee - Svelte for each</summary>

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
<summary markdown="span">svif - Svelte if</summary>

```ts
{#if $1}
   $0
{/if}
$0
```
</details>
    

<details>
<summary markdown="span">svife - Svelte if else</summary>

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
<summary markdown="span">svawait - Svelte await</summary>

```ts
{#await $1}
   {$2}
{:then $3}
   {$4}
{/await}
$0
```
</details>
    

<details>
<summary markdown="span">svkey - Svelte key</summary>

```ts
{#key $1}
   $2
{/key}
$0
```
</details>
    
    

## Note

The snippets include "$1", "$2"... which are placeholders for the cursor position. You can use the tab key to jump between them.

These snippets do not include required imports. You will need to add them yourself.

## License

MIT