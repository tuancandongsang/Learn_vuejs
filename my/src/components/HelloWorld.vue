<template>
  <div>
    <ul>
      <h1>Loop array</h1>
      <li v-for="(item, index) of items" :key="index">
        {{ index }} - {{ item.name }}
      </li>
    </ul>

    <ul >
      <h1>Loop Object</h1>
      <li v-for="(value, key) in object" :key="key">
        {{key}} : {{ value }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      items: [{ name: "Cà phê" }, { name: "Trà đặc" }, { name: "Bò húc" }],
      object: {
        // tất nhiên chúng ta đều biết ông Bành Tổ không phải
        // họ Bành tên Tổ, nhưng đây chỉ là một ví dụ…
        age: 20,
        name: "henrry",
        add: "Hai Duong",
      },
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
