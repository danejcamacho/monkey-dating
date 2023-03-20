<script>
    import {onMount} from 'svelte'
    export let src;

    let loaded = false;
    let failed = false;

    onMount(() => {
      const img = new Image();
			img.src = src;
			
      img.onLoad = () => {
        loaded = true
      }

      img.onerror = () => {
        loaded = false;
				failed = true;
			};


    })
</script>
    
{#if loaded}
<img src = {src} alt="Document" />
{:else if failed}
<img src="/noProfilePic.jpg" alt="Not Found" />
{/if}

<style>
  img {
    width: 200px;
    height: 200px;
    border-radius: 50%;
    object-fit: cover;
    margin-bottom: 20px;
}

</style>

