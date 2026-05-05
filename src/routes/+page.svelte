<script lang="ts">
  import rawBlocks from '$lib/doc.blocks.json';
  import DocRenderer from '$lib/components/DocRenderer.svelte';
  import type { Block } from '$lib/components/DocRenderer.svelte';
  const blocks = rawBlocks as Block[];
</script>



<!-- 
Hard-code custom code that should appear BEFORE Google Doc here. 
This code is in +page.svelte and can be manually coded using HTML or Svelte tags.
-->
<header class="container-fluid d-flex flex-column align-items-end justify-content-center vh-100 mb-4" style="background-image:url('cover.jpg');background-size:cover;background-position:center;padding-right:5%;">
  <div class="col-6 text-end pe-4">
    <h1 class="text-dark display-3" style="text-shadow: 2px 2px 10px rgba(255,255,255,0.9);">Doctors routinely deny Pakistani women their reproductive rights</h1>
    <p class="text-dark fw-light text-center fs-4" style="text-shadow: 2px 2px 10px rgba(255,255,255,0.9);">By Minahil Arif</p>
    <p class="text-dark fw-light text-center fs-6" style="text-shadow: 2px 2px 10px rgba(255,255,255,0.9);">May 5, 2026</p>
  </div>
</header>


<!-- DO NOT EDIT (except to modify classes). This will become code imported from Google Doc. -->
<div class="container">
  <div class="row justify-content-center">
    <div class="col-12 col-sm-10 col-lg-8 col-xxl-6">
      <DocRenderer {blocks} />
    </div>
  </div>
</div>


<!-- Hard-code any custom code that should appear AFTER Google Doc below here. -->
<footer class="container-fluid bg-dark text-white p-5">
  <p class="text-center">UC Berkeley 2026</p>
</footer>