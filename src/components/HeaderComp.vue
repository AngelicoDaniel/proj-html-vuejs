<template>
  <header>
    <div class="container h-100">
      <div class="row d-flex justify-content-between align-items-center">

        <div class="col-6 ">
          <ul class="my-2">
            <li>
              <span><i class="fa-solid fa-clock"></i> Open Hours:
              Mon-Sat-9:00-18:00</span>
            </li>
          </ul>
        </div>

        <div class="col-6">
          <ul class="d-flex justify-content-around m-auto">
            <li>
              <span><i class="fa-solid fa-phone"></i></span>+1(305) 1234-5678
            </li>
            <li>
              <span><i class="fa-solid fa-envelope"></i></span> hello@example.com
            </li>
            <li>
              <span><a href="#"><i class="fa-brands fa-facebook-f"></i></a></span>
            </li>
            <li>
              <span><a href="#"><i class="fa-brands fa-twitter"></i></a></span>
            </li>
            <li>
              <span><a href="#"><i class="fa-brands fa-linkedin-in"></i></a></span>
            </li>
          </ul>
        </div>
        
      </div>
    </div>

  </header>
</template>

<script>
export default {
  name: 'HeaderComp',

}
</script>


<style scoped lang="scss">
header{
  background-color: #21333e;
  height: 5vh;
  color: lightgray;
  i{
   color: lightgray; 
  }
}
</style>
