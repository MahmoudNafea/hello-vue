<template   >
  <div class="container">
    <h2>Home</h2>
    <!-- {{message}} -->
    <span v-bind:title="message">Hover over</span>
    <br />
    <span v-if="seen">See more</span>
    <form>
      <input type="text" placeholder="Add something" />
      <button v-on:click="addItemHandler">Add Item</button>
    </form>
    <ol>
      <AddItem v-for="item in groceryList" v-bind:item="item" v-bind:key="item.key"></AddItem>
    </ol>
  </div>
</template>

<script>
import AddItem from "./../components/AddItem";

export default {
  name: "Home",
  components: { AddItem },
  data() {
    return { message: "Hi", seen: true };
  },
  methods: {
    addItemHandler(e) {
      e.preventDefault();
      console.log("added");
    }
  }
};
</script>
