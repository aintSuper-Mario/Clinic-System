<template>

    <div id="grid">
        <div class="side-nav">
            <h5>Dashboard</h5>
            <ul>
                <li><router-link :to="{name: 'dashboard'}">Home</router-link></li>
                <li><router-link :to="{name: 'patients'}">Patients</router-link></li>
                <li><router-link :to="{name: 'doctors'}">Doctors</router-link></li>
                <li><router-link :to="{name: 'medicines'}">Medicines</router-link></li>
                <li class="logout">Logout</li>
            </ul> 
        </div>
    
        <div class="header">
            <h1>Doctors</h1>
        </div>
    </div>
    
    </template>
    <style>
    #grid{
        display: grid;
        grid-template-columns: repeat(10, 1fr);
        grid-auto-rows: minmax(100px, auto);
    }
    .side-nav{
        color: white;
        background: #0146ae;
        grid-column: 1 / 2;
        grid-row: 1 / 7;
        width: 240px;
    }
    .side-nav h5 {
        text-transform: uppercase;
        font-weight: 800;
        margin: 20px 0 40px 40px;
    }
    .side-nav ul li {
        list-style: none;
        margin: 0  0 40px 20px;
        font-weight: 500;
    }
    .side-nav ul li:hover {
        cursor:pointer;
        font-weight: 800;
    }
    .header {
        grid-column: 2 / 11;
        margin: 20px 0 20px 20px;
    }
    .header h1 {
        font-weight: 900;
    }
    .router-link-exact-active {
        font-weight: 1000;
        text-decoration: underline;
    }
    .side-nav ul .logout {
        margin-left: 40px;
        margin-top: 200px;
        font-weight: 700;
        background: white;
        width: fit-content;
        color: #0146ae;
        padding: 5px;
        border-radius: 6px;
    }
    .side-nav ul .logout:hover {
        box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px, rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px, rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
    }
    </style>