<script>
  import Profile from "./Profile.svelte";
  import Stories from "./Stories.svelte";
  import Footer from "./Footer.svelte";

  export let nickname, name;

</script>

<!-- Sidebar.svelte -->
<style>
  .Sidebar {
    position: relative;
    padding: 4.5em 0 0 0;
  }
  .Sidebar-container {
    position: fixed;
  }

  @media screen and (max-width: 1000px) {
    .Sidebar {
      padding: 3em 4em 0px 4em;
      grid-area: Sidebar
    }

    .Sidebar-container {
      position: relative;
    }

  } 

</style>

<div class="Sidebar">
  <div class="Sidebar-container">
    <Profile {nickname} {name} />
    <Stories />
    <Footer />
  </div>
</div>