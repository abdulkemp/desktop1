<template>
  <div>
    <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
      <div class="modal-dialog modal-xl">
        <div class="modal-content">
          <div class="modal-header">
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
          <div class="modal-body">
            <iframe src="http://www.google.com/search?igu=1" frameborder="0"></iframe>
          </div>
        </div>
      </div>
    </div>
    <div class="modal fade" id="spotify" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="staticBackdropLabel" aria-hidden="true">
      <div class="modal-dialog modal-xl">
        <div class="modal-content">
          <div class="modal-header">
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
          <div class="modal-body" style="background-color:rgb(39, 39, 39)">
            <iframe title="Spotify Embed: Recommendation Playlist "
              src="https://open.spotify.com/embed/playlist/6NW4DkIsHOoNymv5TJEXqC?utm_source=generator&theme=0"
              frameBorder="1" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
              loading="lazy"></iframe>
          </div>
        </div>
      </div>
    </div>
    <div class="modal fade" id="googlerep" data-bs-backdrop="static" data-bs-keyboard="false" tabindex="-1" aria-labelledby="staticBackdropLabel" aria-hidden="true">
      <div class="modal-dialog modal-xl">
        <div class="modal-content">
          <div class="modal-header">
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
          </div>
          <div class="modal-body">
            <iframe src="https://googlerep.netlify.app" frameborder="0"></iframe>
          </div>
        </div>
      </div>
    </div>
    <Folders />
  </div>
</template>

<script>
import Folders from "../components/Folders.vue";
export default {
  name: "Home",
  components: {
    Folders,
  },

};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.modal-content {
  width: 100%;
  height: 100%;
  border-radius: 12px;
}

.modal-body {
  padding: 0;
  background-color: black;
  border-radius: 0 0 10px 10px;
}

.modal-header {
  padding: 8px;
  background-color: rgb(168, 167, 167);
  border-radius: 10px 10px 0 0;
}

.modal-header button {
  background-color: red;
  border-radius: 0 10px 0 0;
  color: black;
  width: 20px;
}

.modal-dialog {
  width: 100%;
  height: 90%;
  /* border-radius: 50px; */
}

iframe {
  width: 100%;
  height: 100%;
  /* border-radius: 0 0 10px 10px; */
  /* background-color: red; */
}

/* .modal{
  position: absolute;
} */
</style>