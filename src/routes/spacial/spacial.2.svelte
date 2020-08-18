<script>
  let src = [
    "/img/spatial/spatial_exemplar_2_1.jpeg",
    "/img/spatial/spatial_exemplar_2_2.jpeg",
    "/img/spatial/spatial_exemplar_2_3.jpeg",
    "/img/spatial/spatial_exemplar_2_4.jpeg",
    "/img/spatial/spatial_exemplar_2_5.jpeg",
    "/img/spatial/spatial_exemplar_2_6.jpeg",
    "/img/spatial/spatial_exemplar_2_7.jpeg",
    "/img/spatial/spatial_exemplar_2_8.jpeg",
    "/img/spatial/spatial_exemplar_2_9.jpeg",
    "/img/spatial/spatial_exemplar_2_10.jpeg",
    "/img/spatial/spatial_exemplar_2_11.jpeg",
    "/img/spatial/spatial_exemplar_2_12.jpeg"
  ];

  let image = 0;

  function nextPhoto() {
    if (image < 11) {
      image++;
    } else if (image >= 11) {
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

<h1 class="title">Spatial Design Example 2</h1>

<img src={src[image]} alt="example2 photos" />

<button class="button is-light" on:click={nextPhoto}>Next</button>
