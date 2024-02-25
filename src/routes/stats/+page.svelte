<!-- Stat.svelte -->

<script>
    import { onMount } from 'svelte';
    
    let responseText = '';
    let isLoading = true;
  
    async function fetchData() {
      try {
        const apiKey = 'ada03af2-fde7-4deb-8019-daf62be2df1e';
        const response = await fetch('https://api.balldontlie.io/v1/stats', {
          headers: {
            'Authorization': `${apiKey}`
          }
        });
        responseText = await response.text();
        isLoading = false;
      } catch (error) {
        console.error('Error fetching data:', error);
        isLoading = false;
      }
    }
  
    onMount(fetchData);
  </script>
  
  {#if isLoading}
    <p>Loading...</p>
  {:else}
    <pre>{responseText}</pre>
  {/if}
  