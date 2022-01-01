<script context="module">
  export async function preload() {
    let data = {};
    const response = await this.fetch(
      `https://api-pugstagram.herokuapp.com/?nickname=MiguelAngelMP&name=MiguelAngel`
    );
    data = await response.json();
    return { data };
  }
</script>

<script>
  import Main from "../components/Main.svelte";
  import Sidebar from "../components/Sidebar.svelte";
  import TimeLine from "../components/TimeLine.svelte";
  export let data;
</script>

<svelte:head>
  <title>PugsTagram</title>
</svelte:head>

<Main>
  <TimeLine posts={data.posts} />
  {#if data.user}
    <Sidebar {...data.user} />
  {/if}
</Main>
