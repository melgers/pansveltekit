<script lang="ts">
  import "../app.postcss";

  // Floating UI for Popups
  import {
    computePosition,
    autoUpdate,
    flip,
    shift,
    offset,
    arrow,
  } from "@floating-ui/dom";
  import { storePopup } from "@skeletonlabs/skeleton";
  storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });
</script>



<div class="flex">
	<div class="w-1/6"></div>
	<div class="w-4/6">
		<slot/>
	</div>
	<div class="w-1/6"></div>
</div>

