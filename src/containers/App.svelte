<script>
  import { onMount } from "svelte";
  import Header from "../components/Header.svelte";
  import Main from "../components/Main.svelte";
  import TimeLine from "../components/TimeLine.svelte";
  import SideBar from "../components/SideBar.svelte";

  let data = {};
  const API = "https://kittygram-api.vercel.app/";

  onMount(async () => {
    const response = await fetch(API);
    data = await response.json();
  });
</script>

<div class="app">
  <Header />
  <Main>
    <TimeLine posts={data.posts} />
    <SideBar {...data.user} />
  </Main>
</div>

<style>
  @import url("https://fonts.googleapis.com/css2?family=Lato:wght@300;400&display=swap");
  @import url("https://fonts.googleapis.com/css2?family=Pacifico&display=swap");

  :global(body) {
    background-color: #fafafa;
    color: rgba(38, 38, 38, 0.7);
    font-family: "Lato", sans-serif;
    /* font-family: 'Pacifico', cursive; */
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  :global(h1, h2, h3) {
    margin: 0;
    padding: 0;
  }
</style>
