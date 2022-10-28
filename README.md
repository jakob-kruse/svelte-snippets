# Svelte Snippets

Snippets for Svelte and Svelte-Kit (using TypeScript)

## Snippets

### Svelte

<details>
  <summary markdown="span">svts - Svelte Script Tag with typescript</summary>

    <script lang="ts">
        $1
    </script>

</details>

<details>
  <summary markdown="span">svdisp - Svelte Event Dispatcher (No Types)</summary>

    const dispatch = createEventDispatcher()
    $0

</details>

<details>
  <summary markdown="span">svdispt - Svelte Event Dispatcher with types</summary>

    const dispatch = createEventDispatcher<{ $1: $2 }>()", "$0"

</details>

<details>
  <summary markdown="span">svhead - Svelte Head Tag with title and description</summary>

    <svelte:head>
        <title>$1</title>
        <meta name="description" content="$2">
    </svelte:head>
    $0

</details>

<details>
  <summary markdown="span">svfe - Svelte For Each</summary>

    {#each $1 as $2 ($3)}
        $0
    {/each}

</details>

<details>
  <summary markdown="span">svfee - Svelte For Each with else</summary>

    {#each $1 as $2 ($3)}
        $4
    {:else}
        $5
    {/each}
    $0

</details>

<details>
  <summary markdown="span">svif - Svelte If</summary>

    {#if $1}
        $2
    {/each}
    $0

</details>

<details>
  <summary markdown="span">svife - Svelte If Else</summary>

    {#if $1}
        $2
    {:else}
        $3
    {/each}
    $0

</details>

### SvelteKit

<details>
  <summary markdown="span">skload - Svelte Kit Server Page Load</summary>

    export const load: PageServerLoad = async ({ $1 }) => {
        return {
            $2
        };
    };

</details>

<details>
  <summary markdown="span">skactions - Svelte Kit Form Actions</summary>

    export const actions: Actions = {
        async default({ $1 }) {
            $2
            return {
                $3
            };
        }
    };

</details>

## Note

The snippets include "$1", "$2"... which are placeholders for the cursor position. You can use the tab key to jump between them.

These snippets do not include required imports. You will need to add them yourself.
