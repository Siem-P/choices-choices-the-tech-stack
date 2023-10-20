<script setup>
const data = fetch("http://localhost:8055/items/articles")
  .then((response) => response.json())
  .then((data) => {
    console.log(data);
  })
  .catch((error) => {
    console.error(error);
  });

console.log(data);
</script>