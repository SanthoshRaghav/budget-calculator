<script>
    //components
    import Navbar from './Navbar.svelte';
    import Title from './Title.svelte';

    //data
    import expenseData from './expenses';

    //variables
    let expenses=[...expenseData];
    console.log(expenses);
</script>

<style></style>

<Navbar/>
<Title title="add expenses"/>