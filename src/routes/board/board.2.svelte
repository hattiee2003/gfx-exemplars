<script>
  let src = [
    "/img/board/board_exemplar_2_1.jpeg",
    "/img/board/board_exemplar_2_2.jpeg",
    "/img/board/board_exemplar_2_3.jpeg",
    "/img/board/board_exemplar_2_4.jpeg",
    "/img/board/board_exemplar_2_5.jpeg",

  ];

  let image = 0;

  function nextPhoto() {
    if (image < 4) {
      image++;
    } else if (image >= 4) {
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

<h1 class="title">Board Design Example 2</h1>

<img src={src[image]} alt="example2 photos" />

<button class="button is-light" on:click={nextPhoto}>Next</button>