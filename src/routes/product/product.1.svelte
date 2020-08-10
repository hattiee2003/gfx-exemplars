<script>
  let src = [
    "/img/product/product_exemplar_1_1.jpeg",
    "/img/product/product_exemplar_1_2.jpeg",
    "/img/product/product_exemplar_1_3.jpeg",
    "/img/product/product_exemplar_1_4.jpeg",
    "/img/product/product_exemplar_1_5.jpeg",
    "/img/product/product_exemplar_1_6.jpeg",
    "/img/product/product_exemplar_1_7.jpeg",
    "/img/product/product_exemplar_1_8.jpeg",
    "/img/product/product_exemplar_1_9.jpeg"
  ];

  let image = 0;

  function nextPhoto() {
    if (image < 8) {
      image++;
    } else if (image >= 8) {
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

<h1 class="title">Product Design Example 1</h1>

<img src={src[image]} alt="example1 photos" />

<button class="button is-light" on:click={nextPhoto}>Next</button>