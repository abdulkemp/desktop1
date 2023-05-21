<template>
    <div>
        <div class="contain">
            <div class="left-folders">
                <div class="desktop">
                    <div class="fold justify-content-start">
                        <div class="forms" style="height: 5rem">
                            <button type="button" data-bs-toggle="modal" data-bs-target="#googlerep">
                                <div class="folder">
                                    <img src="https://i.postimg.cc/k5V07PHW/pngegg-5.png" alt="" />
                                </div>
                                <div class="text">
                                    <p>Recycle Bin</p>
                                </div>
                            </button>
                        </div>
                    </div>
                    <div class="fold justify-content-start">
                        <button type="button" data-bs-toggle="modal" data-bs-target="#exampleModal">
                            <div class="forms">
                                <div class="folder folding">
                                    <img src="https://i.postimg.cc/Ghyxj2WZ/pngwing-com-1.png" alt=""
                                        style="margin-top: 0.5rem" />
                                </div>
                                <div class="text">
                                    <p>Google Chrome</p>
                                </div>
                            </div>
                        </button>
                    </div>
                    <div class="fold justify-content-start">
                        <div class="forms">
                            <div class="folder">
                                <img src="https://i.postimg.cc/rFR2C1FM/pngegg-5.png" alt="" />
                            </div>
                            <div class="text">
                                <p>Visual Studio Code</p>
                            </div>
                        </div>
                    </div>
                    <div class="fold justify-content-start">
                        <div class="forms" style="height: 5rem">
                            <div class="folder">
                                <img src="https://i.postimg.cc/T3H883tR/pngegg-6.png" alt="" />
                            </div>
                            <div class="text">
                                <p>Git Bash</p>
                            </div>
                        </div>
                    </div>
                    <div class="fold justify-content-start">
                        <div class="forms">
                            <div class="folder">
                                <img src="https://i.postimg.cc/YC4KR1rt/pngwing-com.png" alt="" />
                            </div>
                            <div class="text">
                                <p>Microsoft Edge</p>
                            </div>
                        </div>
                    </div>
                    <div class="fold justify-content-start">
                        <button type="button" data-bs-toggle="modal" data-bs-target="#spotify">
                            <div class="forms" style="height: 5rem">
                                <div class="folder spot">
                                    <img src="https://i.postimg.cc/vH0xfdBp/pngwing-com-3.png" alt=""
                                        style="margin-top: 0.5rem" />
                                </div>
                                <div class="text">
                                    <p>Spotify</p>
                                </div>
                            </div>
                        </button>
                    </div>
                </div>
            </div>
            <!-- <div class="fold justify-content-start" v-for="pro in work" :key="pro" >
                <button type="button" data-bs-toggle="modal" data-bs-target="#exampleModal">
                    <div class="forms">
                        <div class="folder folding">
                            <img :src="pro.image" alt="" style="margin-top: 0.5rem" />
                        </div>
                        <div class="text">
                            <p>{{ pro.text }}</p>
                        </div>
                    </div>
                </button>
                <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel"
                    aria-hidden="true">
                    <div class="modal-dialog modal-xl">
                        <div class="modal-content">
                            <div class="modal-header">
                                <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                            </div>
                            <div class="modal-body">
                                <iframe :src="pro.frame" frameBorder="1"
                                    allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
                                    loading="lazy"></iframe>
                            </div>
                        </div>
                    </div>
                </div>
            </div> -->
        </div>
    </div>
</template>
  
<script>
export default {
    name: "Folders",
    data() {
        return {
            work: [
                {
                    text: "Spotify",
                    image: "https://i.postimg.cc/vH0xfdBp/pngwing-com-3.png",
                    frame: "https://open.spotify.com/embed/playlist/6NW4DkIsHOoNymv5TJEXqC?utm_source=generator&theme=0",
                },
                {
                    text: "Google Chrome",
                    image: "https://i.postimg.cc/Ghyxj2WZ/pngwing-com-1.png",
                    frame: "http://www.google.com/search?igu=1",
                },
                {
                    text: "Google Chrome",
                    image: "https://i.postimg.cc/Ghyxj2WZ/pngwing-com-1.png",
                    frame: "http://googlerep.netlify.app",
                },
            ]
        }
    }
};

</script>
  
<style>
.desktop {
    /* border: 3px solid grey; */
    width: 10%;
    display: inline-block;
    justify-content: center;
    align-items: center;
    height: 100%;
    /* margin-top: 1rem; */
    text-align: center;
    margin-left: 7px;
}

.fold {
    display: flex;
    justify-content: center;
    align-items: center;
    max-height: 100%;
}

.folder {
    width: 100%;
    margin-top: 7px;
    /* display: flex;
    justify-content: center;
    align-items: center; */
}

.text {
    padding-top: 5px;
    display: flex;
    justify-content: center;
    align-content: center;
}

.forms:hover {
    background: rgba(128, 128, 128, 0.362);
    border-radius: 5px;
    cursor: pointer;
}



button {
    background: transparent;
    border: none;
}

button a {
    text-decoration: none;
}

.forms {
    /* border: 2px solid ; */
    margin-top: 5px;
    margin-bottom: 5px;
    width: 5rem;
    height: 6rem;
}

.forms p {
    color: white;
}

.forms img {
    width: 2.5rem;
    height: 2.5rem;
}

@media screen and (min-width: 1920px) {
    .spot img {
        margin-top: 1.5rem;
    }

    .desktop {
        margin-top: 1rem;
    }
}
</style>