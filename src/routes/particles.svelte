<script>
    import { onMount } from "svelte";
  
    onMount(() => {
      particlesJS("particles-container", {
        // Particle.js configuration options go here
      });
    });
  </script>
  
  <div id="particles-container"></div>
  
  <style>
    #particles-container {
      position: absolute;
      width: 100%;
      height: 100%;
      z-index: -1;
    }
  </style>
  