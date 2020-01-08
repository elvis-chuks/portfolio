<template>
    <div>
    <img src="../assets/peeps.svg" class="img-fluid" pic>
    </div>
</template>

<script>
export default {
    name: "ExperienceRight"
}
</script>

<style scoped>
[pic]{
  margin-top: 130px;
  /* margin-bottom: 150px; */
}
@media (max-width: 576px) { 
    [pic]{
      margin-left: -18px;
      /* width:450px; */
      margin-bottom: 150px;
      margin-top: 50px;
  }
 }
</style>