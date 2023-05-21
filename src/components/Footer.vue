<template>
    <div class="footer">
        <div class="containe fixed-bottom">
            <div class="row">
                <div class="col-4 left">
                    <div class="weather">
                        <div class="humidity">
                            <img src="https://i.postimg.cc/hvLSPKdf/pngegg-1.png" alt="" />
                        </div>
                        <div class="temp">
                            <p class="temperature">14°C</p>
                            <p>Mostly cloudly</p>
                        </div>
                    </div>
                </div>
                <div class="col-4 middle">
                    <div class="col middle-icons">
                        <div class="icons">
                            <img src="https://i.postimg.cc/2yrthW6F/bb6961095e9a6dc1aac2af24ea88fc52.png" alt="" />
                        </div>
                    </div>
                    <div class="bar">
                        <div class="searching">
                            <form @submit.prevent>
                                <input type="search" name="search-outline" id="" placeholder="Search" class="search"
                                    v-model="searchQuery" />
                            </form>
                        </div>
                    </div>
                    <div class="col middle-icons">
                        <div class="icons">
                            <img src="https://i.postimg.cc/ryWvD8hw/pngegg-7.png" alt="" />
                        </div>
                    </div>
                    <div class="col middle-icons">
                        <div class="icons">
                            <img src="https://i.postimg.cc/YC4KR1rt/pngwing-com.png" style="margin-top: 0.1rem" alt="" />
                        </div>
                    </div>
                    <div class="col middle-icons">
                        <div class="icons">
                            <img src="https://i.postimg.cc/8cstGmn5/pngegg-3.png" style="border-radius: 0 0 5px 5px"
                                alt="" />
                        </div>
                    </div>
                    <button type="button" data-bs-toggle="modal" data-bs-target="#exampleModal">
                        <div class="col middle-icons" style="width:2.7rem">
                            <div class="icons" style=" height: 2.4rem; width:2rem">
                                <img src="https://i.postimg.cc/Ghyxj2WZ/pngwing-com-1.png" alt="" />
                            </div>
                        </div>
                    </button>
                    <div class="col middle-icons">
                        <div class="icons">
                            <img src="https://i.postimg.cc/rFR2C1FM/pngegg-5.png" alt="" />
                        </div>
                    </div>
                    <div class="col middle-icons">
                        <div class="icons">
                            <img src="https://i.postimg.cc/gJh3Ht53/pngwing-com-2.png" alt="" />
                        </div>
                    </div>
                    <button type="button" data-bs-toggle="modal" data-bs-target="#staticBackdrop">
                        <div class="col middle-icons" style="width:2.7rem">
                            <div class="icons" style=" height: 2.4rem; width:2rem">
                                <img src="https://i.postimg.cc/vH0xfdBp/pngwing-com-3.png" alt="" />
                            </div>
                        </div>
                    </button>
                    <div class="col middle-icons">
                        <div class="icons">
                            <img src="https://i.postimg.cc/qMW09mZN/pngegg-4.png" alt="" />
                        </div>
                    </div>
                </div>
                <div class="col-4 right">
                    <div class="col size">
                        <div class="set">
                            <img src="https://i.postimg.cc/R0QVwjQk/pngegg-15.png" style="width: 12px; height: 12px"
                                alt="" />
                            <img src="https://i.postimg.cc/RFSCdXgN/pngegg-16.png" style="width: 15px; height: 12px"
                                alt="" />
                            <img src="https://i.postimg.cc/W4P1F2rm/pngegg-17.png" style="width: 23px; height: 23px"
                                alt="" />
                        </div>
                    </div>
                    <div class="col size">
                        <div class="lang text-center">
                            <p style="color: black">ENG</p>
                            <p style="color: black">US</p>
                        </div>
                    </div>
                    <div class="col size">
                        <div class="settings">
                            <img src="https://i.postimg.cc/HkNLpwWN/pngegg-8.png" alt="" />
                            <img src="https://i.postimg.cc/JhBztsGz/pngegg-9.png" style="margin-left: 7px" alt="" />
                            <img src="https://i.postimg.cc/W1z3LWVr/pngegg-10.png" style="margin-left: 7px" alt="" />
                        </div>
                    </div>
                    <div class="t-n">
                        <div class="col size time-noti">
                            <div class="time text-end">
                                <p style="color: black">00:42</p>
                                <p style="color: black">2023/05/14</p>
                            </div>
                            <div class="noti">
                                <img src="https://i.postimg.cc/bwZtHNsK/pngegg-14.png" alt="" />
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
  
<script>
export default {
    name: "Footer",
};
</script>
  
<style>
.containe {
    /* background-image: linear-gradient, white); */
    background: rgba(191, 237, 251, 0.503);
    backdrop-filter: blur(12px);
    width: 100%;
}

.row {
    border-top: 1px solid rgba(120, 149, 153, 0.253);
    height: 3.5rem;
}

.left {
    width: 24%;
    display: flex;
    justify-content: start;
    align-items: center;
}

.right {
    width: 25%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.middle {
    width: 51%;
    display: flex;
    justify-content: center;
    align-content: center;
}

.search {
    width: 75vh;
    height: 44px;
    border-radius: 50px;
    border: transparent;
    /* text-align: center; */
    padding-left: 30px;
    padding-right: 30px;
    font-size: 15px;
    color: rgb(94, 94, 94);
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}

.middle-icons {
    display: flex;
    justify-content: center;
    align-content: center;
    margin: 0.3rem;
    /* border: 1px solid black; */
}

.middle-icons:hover {
    background: rgba(255, 255, 255, 0.555);
    border-radius: 3px;
    cursor: pointer;
}

.size {
    /* margin: 0.3rem; */
    height: 2.7rem;
    display: flex;
    justify-content: center;
    align-content: center;
}

.size:hover {
    background: rgba(255, 255, 255, 0.555);
    border-radius: 3px;
    cursor: pointer;
}

.icons {
    display: flex;
    justify-content: center;
    align-content: center;
    margin-top: 0.5rem;
    width: 2.6rem;
}



.icons:active {
    border-bottom: 2px solid blue;
    border-bottom-width: 2px;
}

.icons:hover {
    border-bottom: 2px solid blue;
    border-bottom-width: 2px;
}

/* .icons:hover {
      border-bottom: 2px solid blue;
      border-bottom-width: 2px;
  } */

.time-noti {
    display: flex;
    justify-content: center;
    align-items: center;
    /* border: 1px solid black; */
    margin-right: 1rem;
}

.t-n {
    width: 8rem;
}

.search {
    width: 13rem;
    height: 2.1rem;
    border-radius: 50px;
    background: rgba(179, 242, 250, 0.459);
    border: 1px solid rgba(90, 117, 126, 0.281);
}

.bar {
    margin-top: 0.7rem;
}

p {
    height: 2px;
    font-size: 12px;
    color: grey;
}

.temperature {
    font-weight: 700;
    color: black;
}

.temp {
    margin-left: 6px;
}

.weather {
    display: flex;
    justify-content: start;
    align-items: center;
    width: 10rem;
    height: 40px;
    margin-left: 0.7em;
}

.weather:hover {
    background: rgba(255, 255, 255, 0.555);
    border-radius: 3px;
    cursor: pointer;
}

.weather img {
    width: 2rem;
}

.middle-icons img {
    width: 1.7rem;
    height: 1.7rem;
}

.settings img {
    width: 1.2rem;
    height: 1.2rem;
    /* margin-left: 6px; */
}

.settings {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 6rem;
    /* height: 2rem; */
    margin-left: 1px;
}

.noti {
    display: flex;
    justify-content: start;
    align-items: center;
    margin-left: 0.6rem;
}

.noti img {
    width: 1.2rem;
    height: 1.2rem;
    /* margin-left: 6px; */
}

.set {
    display: flex;
    justify-content: end;
    align-items: center;
    width: 6rem;
}

.set img {
    margin-right: 0.5rem;
    /* margin-left: 6px; */
}

@media screen and (min-width: 1920px) {
    .left {
        width: 24%;
        display: flex;
        justify-content: start;
        align-items: center;
    }

    .right {
        width: 22%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .middle {
        width: 54%;
        display: flex;
        justify-content: center;
        align-content: center;
    }

    .middle-icons {
        width: 8rem;
    }
}</style>