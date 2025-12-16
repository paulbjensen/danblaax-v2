<script lang="ts">
  import { Slidy, type Slide } from "@slidy/svelte";
  import "@slidy/svelte/dist/slidy.css";

  export let slides: Slide[] = [];
  export let options = {
    arrows: true,
    navigation: false,
    progress: false,
    thumbnail: true,
    counter: false,
  };
</script>

<Slidy {slides} {...options} />