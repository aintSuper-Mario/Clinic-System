<script>
import Agenda from '../components/Agenda.vue'
export default {
    components: {Agenda}
}
</script>

<template>
    <div class="wrapper">
        <div class="description-wrapper">
            <h1 class="mb-3">HealthHub Clinic Booking Appointment</h1>
        </div>
        <hr>
        <div class="booking-container">
            <div class="booking-content">
                <h2 class="mt-5">Personal Information</h2>
                <form>
                    <label>Full Name:</label> <br>
                    <input type="text" placeholder="Last Name" required> <br> <br>
                    <input type="text" placeholder="First Name" required>
                    <br> <br>
                    <label>Gmail:</label> <br>
                    <input type="email" placeholder="Gmail" required>
                    <button type="submit" class="btn btn-primary mt-4">Submit</button>
                </form>
                <hr>
                <div class="agenda">
                    <Agenda />
                    <hr>
                </div>

            </div>
        </div>
    </div>


    <!-- para booking wrapper -->
    <!-- :after {
        content: "";
        display: block;
        clear: left;
        margin-bottom: 50px;
    } -->

</template>

<style scoped>
.wrapper {
    margin: 50px 200px;
}

.description-wrapper:after {
    content: "";
    display: block;
    clear: both;
    margin-bottom:  60px;

}
.description-wrapper h1 {
    font-weight: 900;
    color: #0146ae;
    font-size: 2.5rem;
}

p {
    font-weight: 500;
    line-height: 30px;
}

.booking-information {
    border-radius: 20px;
    box-shadow: rgba(50, 50, 93, 0.25) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
    width: 180px;
    height: 180px;
    padding: 10px;
    float: left;
    background: #474bff;
background: -webkit-linear-gradient(0deg, #474bff 0%, #0146ae 100%);
background: linear-gradient(0deg, #474bff 0%, #0146ae 100%);
}

ul {
    display: flex;
    flex-direction: column;
    align-items: stretch;
}

li {
    font-size: 16px;
    font-weight: 600;
    margin: 15px 0;
    color: white;

}

li:hover {
    text-decoration: underline;
    font-weight: 700;
}

.booking-wrapper {
    margin-right: 400px;
}

.booking-container {

    text-align: justify;
}

.booking-container form input {
    width: 100%;
    padding: 1%;
}

h2 {
    margin-bottom: 20px;
    color: #0146ae;
    font-weight: 800;
}

form {
    margin-bottom: 30px;
}

span {
    font-weight: bold;
    color: #ff0062;
}
.calendar-container table {
    margin: 0 auto;
}
label {
font-weight: bold;
}
input {
    border-radius: 4px;
    border: 1px solid #474bff;
}

input:focus {
outline: none;
}
table tr th, td {
    margin-right: 20px;
}

table {
    padding: 10px;
    border-radius: 4px;
    font-size: 25px;
    width: 100%;
    height: 200px;
    color: white;
}
h3 {
    font-weight: 700;
}
button {
    width: 150px;
    height: 50px;
}
h5 {
    margin-top: 20px;
    display: inline-block;
    margin-right: 20px;
}

.red {
    background-color: #ff0062;
    padding: 10px;
    width: 180px;
    border-radius: 4px;
}

.green {
    background-color:rgb(23, 190, 23);
    padding: 10px;
    width: 180px;
    border-radius: 4px;
}
.schedules {
    float: right;
    position: relative;
    bottom: 350px;
    left: 420px;
    background: #474bff;
background: -webkit-linear-gradient(0deg, #474bff 0%, #0146ae 100%);
background: linear-gradient(0deg, #474bff 0%, #0146ae 100%);
color: white;
width: 45%;
border-radius: 4px;
padding: 2%;
}
h6 {
    font-weight: 700;
}
</style>