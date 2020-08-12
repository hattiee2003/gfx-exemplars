<script>
  let src = [
    "/img/spatial/spatial_exemplar_1_1.jpeg",
    "/img/spatial/spatial_exemplar_1_2.jpeg",
    "/img/spatial/spatial_exemplar_1_3.jpeg",
    "/img/spatial/spatial_exemplar_1_4.jpeg",
    "/img/spatial/spatial_exemplar_1_5.jpeg",
    "/img/spatial/spatial_exemplar_1_6.jpeg",
    "/img/spatial/spatial_exemplar_1_7.jpeg",
    "/img/spatial/spatial_exemplar_1_8.jpeg",
    "/img/spatial/spatial_exemplar_1_9.jpeg",
    "/img/spatial/spatial_exemplar_1_10.jpeg",
    "/img/spatial/spatial_exemplar_1_11.jpeg",
    "/img/spatial/spatial_exemplar_1_12.jpeg",
    "/img/spatial/spatial_exemplar_1_13.jpeg"
  ];

  let image = 0;

  function nextPhoto() {
    if (image < 12) {
      image++;
    } else if (image >= 12) {
      image = 0;
    }
  }
</script>

<style>
  img {
    height: 440px;
    width: auto;
    display: block;
    margin-left: auto;
    margin-right: auto;
    padding: 10px;
  }

  button {
    display: block;
    margin-left: auto;
    margin-right: auto;
    background-color: #3D405B !important;
    color: white !important;
  }

  button:hover{
    background-color: rgb(101, 106, 148) !important;
    color: white !important;
  }
</style>

<h1 class="title">Spacial Design Example 1</h1>

<img src={src[image]} alt="example1 photos" />

<button class="button is-light" on:click={nextPhoto}>Next</button>
