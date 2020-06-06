<template>
  <div>
    <h2>This's add item component</h2>
    <li>{{items.text}}</li>
  </div>
</template>

<script>
export default {
  name: "AddItem",
  props: ["items"],
  data() {
    return {
      groceryList: [
        { id: 0, text: "veg" },
        { id: 1, text: "veg" },
        { id: 2, text: "veg" }
      ]
    };
  }
};
</script>