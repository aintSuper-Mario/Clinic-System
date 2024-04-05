<template>
    <div class="about mt-3  rounded">
        <h2 class="text-center">Explore our Services</h2>
    </div>
    
      <div class="card-container mb-5">
        <router-link :to="{name: 'eyeService'}"><div class="card">
            <img class="card-img-top" src="../assets/images/services1.jpg" alt="Card image cap">
          <div class="card-header text-center">Your Clear Vision Partner: Expert Ophthalmology Care at HealthHub</div>
          <div class="card-body border rounded">
            <p class="card-text">
                Experience exceptional eye care with our skilled ophthalmologist. Our specialist is committed to preserving and enhancing your vision through personalized, state-of-the-art treatments. From routine check-ups to advanced surgical procedures, trust us for compassionate eye care.
            </p>
          </div>
        </div></router-link>
       <router-link :to="{name: 'enService'}"><div class="card"> 
          <img class="card-img-right" src="../assets/images/services2.jpg" alt="Card image cap" height="">
          <div class="card-header text-center">
            Complete EN Care: Your Trusted Otolaryngologist at HealthHub
          </div>
          <div class="card-body border rounded">
            <p class="card-text">
              Experience comprehensive care for your ears and nose with our expert otolaryngologist. At HealthHub, our specialist is dedicated to diagnosing and treating a wide range of EN conditions. From hearing issues to sinus disorders, trust us for personalized and advanced EN care.
            </p>
          </div>
        </div></router-link>
      </div>
</template>

<script>

</script>

<style scoped>
.about {
    background-color: #0146ae;
    text-transform: uppercase;
    width: fit-content;
    margin: 50px auto;
    border: 1px solid whitesmoke;
    color: white;
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
    padding: 7px 20px;
    cursor: pointer;
}

.about h2 {
    font-weight: bold;
}


.card-container {
    justify-content: space-around;
    margin-top: 40px;
    display: flex;
    flex-direction: row;
}

.card-container .card {
    width: 450px;
    height: 300px;

}

.card-container .card:hover {
    cursor: pointer;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
}

.card-header {
    background-color: #0146ae;
    color: #eee;
    font-weight: bold;
}
.card-body {
    border: 1px solid #0146ae;
}

.card-text {
    text-align: justify;
}

a {
  text-decoration: none;
}
</style>