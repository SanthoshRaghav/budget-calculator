<script>
    //components
    import Navbar from './Navbar.svelte';
    import Title from './Title.svelte';
    import ExpensesList from './ExpensesList.svelte';

    //data
    import expenseData from './expenses';

    //variables
    let expenses=[...expenseData];

    //functions
    function removeExpense(id){
        expenses=expenses.filter(item=>item.id!==id)
    }
</script>

<style></style>

<Navbar/>
<main class="content">
    <ExpensesList {expenses} {removeExpense}/>
</main>