<script>
  let src = [
    "/img/product/product_exemplar_3_1.jpeg",
    "/img/product/product_exemplar_3_2.jpeg",
    "/img/product/product_exemplar_3_3.jpeg",
    "/img/product/product_exemplar_3_5.jpeg",
    "/img/product/product_exemplar_3_6.jpeg",
    "/img/product/product_exemplar_3_7.jpeg",
    "/img/product/product_exemplar_3_9.jpeg"
  ];

  let image = 0;

  function nextPhoto() {
    if (image < 6) {
      image++;
    } else if (image >= 6) {
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

<h1 class="title">Product Design Example 3</h1>

<img src={src[image]} alt="example3 photos" />

<button class="button is-light" on:click={nextPhoto}>Next</button>