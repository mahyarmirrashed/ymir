<script lang="ts">
  import "../app.css";
  import { i18n } from "$lib/i18n";
  import { ParaglideJS } from "@inlang/paraglide-sveltekit";
  let { children } = $props();

  export const prerender = true;
  export const ssr = false;
</script>

<ParaglideJS {i18n}>
  {@render children()}
</ParaglideJS>
