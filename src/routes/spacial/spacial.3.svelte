<script>
  let src = [
    "/img/spatial/spatial_exemplar_3_1.jpeg",
    "/img/spatial/spatial_exemplar_3_2.jpeg",
    "/img/spatial/spatial_exemplar_3_3.jpeg",
    "/img/spatial/spatial_exemplar_3_4.jpeg",
    "/img/spatial/spatial_exemplar_3_5.jpeg",
    "/img/spatial/spatial_exemplar_3_6.jpeg",
    "/img/spatial/spatial_exemplar_3_10.jpeg",
    "/img/spatial/spatial_exemplar_3_11.jpeg",
    "/img/spatial/spatial_exemplar_3_12.jpeg",
    "/img/spatial/spatial_exemplar_3_13.jpeg"
  ];

  let image = 0;

  function nextPhoto() {
    if (image < 9) {
      image++;
    } else if (image >= 9) {
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
  }
</style>

<h1 class="title">Spacial Design Example 3</h1>

<img src={src[image]} alt="example3 photos" />

<button class="button is-light" on:click={nextPhoto}>Next</button>