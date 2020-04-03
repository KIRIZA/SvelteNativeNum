<flexboxLayout class='flex-centered'>
    <label class='h1 text-center' text='page 3' />
        <cardView margin='32' elevation='40'>
            <button text='page 2' on:tap = { () => selectedTab = 0 } />
        </cardView>
</flexboxLayout>

<script>
//    import Chart from './Chart.svelte';
    export let selectedTab
    let data = [1,2,3,4,5,6]
</script>

<stackLayout>
    <textField type="number" bind:text={data[0]} />
    <textField type="number" bind:text={data[1]} />
    <textField type="number" bind:text={data[2]} />
    <textField type="number" bind:text={data[3]} />
    <textField type="number" bind:text={data[4]} />
    <textField type="number" bind:text={data[5]} />
</stackLayout>

<!-- <Chart {data} /> -->

