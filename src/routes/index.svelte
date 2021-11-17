<script context="module">
    export async function preload(){
        let data = {};
        const response = await this.fetch(
            `https://api-pugstagram.herokuapp.com/?nickname=MiguelAngelMP&name=Miguel%20Ange`
        );
        data = await response.json();
        return { data};
    }
</script>

<script>

    import Header from '../components/Header.svelte';
    import Main from '../components/Main.svelte';
    import Sidebar from '../components/Sidebar.svelte';
    import TimeLine from '../components/TimeLine.svelte';
    export let data;
</script>

<svelte:head>
    <title>Pugstagram</title>
</svelte:head>

<Main>
	<TimeLine posts={data.posts} />
		{#if data.user}
			<Sidebar {... data.user} />
		{/if}
</Main>