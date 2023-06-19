<template>
   
    <div id="footer" class="container mx-auto ">
        <footer class="footer mt-4 rounded-tr-md rounded-tl-md  p-4 bg-white font-medium text-slate-600  shadow flex justify-between">
            <div><span><i class="fa-regular fa-copyright"></i></span> {{ currentYear }}<span><h4>T-Wind</h4></span>
            </div>
            <div>-Crafted by Sumit Shrestha</div>

        </footer>

    </div>

</template>

<script>
export default {
  data() {
    return {
      currentYear: new Date().getFullYear()
    };
  }
};
</script>

<style lang="scss" scoped>

</style>