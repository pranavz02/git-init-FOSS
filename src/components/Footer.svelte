<script>
  import Instagram from 'svelte-icons/fa/FaInstagram.svelte'
  import Facebook from 'svelte-icons/fa/FaFacebookSquare.svelte'
  import LinkedIn from 'svelte-icons/fa/FaLinkedin.svelte'
  import Medium from 'svelte-icons/fa/FaMedium.svelte'
</script>

<main>
  <div class="date">AASF/2022</div>
  <div class="socials">
    <a
      rel="noopener"
      aria-label="Instagram"
      href="https://instagram.com/aasf_iiitmg"
      target="_blank"
      class="icon"><Instagram /></a
    >
    <a
      rel="noopener"
      aria-label="Facebook"
      href="https://www.facebook.com/aasfiiitm/"
      target="_blank"
      class="icon"><Facebook /></a
    >
    <a
      rel="noopener"
      aria-label="LinkedIn"
      href="https://www.linkedin.com/company/aasf-iiitmg"
      target="_blank"
      class="icon"><LinkedIn /></a
    >
    <a
      rel="noopener"
      aria-label="Medium"
      href="https://medium.com/tech-iiitg"
      target="_blank"
      class="icon"><Medium /></a
    >
  </div>
</main>

<style>
  main {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px;
    border-top: 1px solid black;
    padding: 2px;
  }

  :global(body.dark-mode) main{
    border-top: 0.5px solid rgba(255, 255, 255, 0.746);

  }
  
  /* .date{
    color: chartreuse;
  } */
  .socials {
    display: flex;
    gap: 1rem;
  }
  :global(body.dark-mode) .icon{
		color: white;
	}

  .icon{
    height: 40px;
    width: 40px;
    color: rgb(0, 0, 0);
    transition: color 0.7s ease-out, transform 0.7s ease-in-out;
  }
  :global(body.dark-mode) .icon:hover{
    color: #00ff00;
	}
  .icon:hover {
    cursor: pointer;
    color: rgb(5, 153, 5);
    transform: rotate(360deg) scale(1.5);
  }
</style>
