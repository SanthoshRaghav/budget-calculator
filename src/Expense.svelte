<script>
  //packages
  import { getContext } from "svelte";

  //props
  export let id;
  export let name = "";
  export let amount = 0;

  //varibales
  let showAmount = false;

  //functions
  function toggleAmmount() {
    showAmount = !showAmount;
  }

  //context api
  let removeExpense = getContext("remove");
</script>

<article class="single-expense">
  <div class="expense-info">
    <h2>
      {name}
      <button class="amount-btn" on:click="{toggleAmmount}">
        <i class="fas fa-caret-down"></i>
      </button>
    </h2>
    {#if showAmount}
    <h4>amount: ${amount}</h4>
    {/if}
  </div>
  <div class="expense-buttons">
    <button class="expense-btn edit-btn">
      <i class="fas fa-pen"></i>
    </button>
    <button class="expense-btn delete-btn">
      <i class="fas fa-eraser" on:click="{()=>removeExpense(id)}"></i>
    </button>
  </div>
</article>
