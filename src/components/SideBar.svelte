<script>
  import Profile from "./Profile.svelte";
  import Stories from "./Stories.svelte";
  import Footer from "./Footer.svelte";

  export let nickname;
  export let name;
</script>

<section class="SideBar">
  <div class="SideBar-container">
    <Profile />
    <Stories {nickname} {name} />
    <Footer />
  </div>
</section>

<style>
  .SideBar {
    position: relative;
    padding: 4.5em 0 0 0;
  }
  .SideBar-container {
    position: fixed;
  }
</style>
