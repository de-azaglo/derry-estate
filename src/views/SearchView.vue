<template>
    <main class="search">
        <h2>Find Your Dream Home</h2>
        <p>Now you can save on all stree, time, and hidden costs, with hundreds of homes for you</p>

        <div class="search-container">
            <div class="filter-container">
                <button class="filter first">Buy</button>
                <button class="filter middle">Rent</button>
                <button class="filter last">New Property</button>
            </div>

            <div class="search-box">
                <div class="left-side">
                <div class="search-option">
                    <i class='bx bx-home'></i>
                    <p>House Type</p>
                    <i class='bx bx-chevron-down' ></i>
                </div>
                <div class="search-option">
                    <i class='bx bx-money'></i>
                    <p>Price Range</p>
                    <i class='bx bx-chevron-down' ></i>
                </div>
                <input type="text" placeholder="Search for your dream home" class="search-option"/>
                </div>
                <button>Search</button>
            </div>
        </div>
    </main>
</template>

<style>

 .search{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background: url(/src/assets/pictures/search-home.svg) no-repeat;
    background-size: cover;
 }

 .search h2{
    font-size: 4em;
    font-weight: 800;
    color: white;
 }

 .search p{
    color: white;
    font-size: 1.1em;
 }

 .search-container{
    margin-top: 9vh;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    width: 70vw;
 }

 .filter-container{
    /* background-color: white; */
    background-color: rgba(255, 255, 255, 0.4); /* set background opacity to 50% */
    padding: 0;
    border-radius: 10px 10px 0 0;
    width: auto;
 }

 .filter-container button{
    background-color: transparent;
    border: none;
    /* border-radius: 10px 10px 0 0; */
    font-size: 1.3em;
    padding: 8px 12px;
 }

 .first{
    border-radius: 10px 0 0 0;
 }
 .middle{
    border-radius: 0;
 }
 .last{
    border-radius: 0 10px 0 0;
 }

  .filter-container button:hover{
    background-color: rgba(255, 255, 255, 0.7);
    color: var(--vt-c-green);
 }

 .search-box{
    display: flex;
    width: 100%;
 }

 .search-box .left-side{
    background-color: rgba(255, 255, 255, 0.7);
    display: flex;
    width: 100%;
    border-radius: 0 0 0 10px;
 }

 .search-option{
    display: flex;
    align-items: center;
    padding: 25px 12px;
    color: var(--vt-c-green);
 }

 .search-option p{
    font-size: 1.3em;
    color: var(--vt-c-green);
    margin: 0 6px;
 }

 .search-option i{
    font-size: 1.3em;
 }

 .search-box input{
    border: none;
    background-color: transparent;
    width: 53%;
 }
 
 .search-box input::placeholder{
    color: var(--vt-c-green);
    font-size: 1.3em;
 }

 .search-box button{
    background-color: var(--vt-c-green);
    color: white;
    border: none;
    padding: 20px 15px;
    font-size: 1.3em;
    cursor: pointer;
 }
</style>