<script>
  let src = [
    "/img/board/board_exemplar_3_1.jpeg",
    "/img/board/board_exemplar_3_2.jpeg",
    "/img/board/board_exemplar_3_3.jpeg",
    "/img/board/board_exemplar_3_4.jpeg",
  ];

  let image = 0;

  function nextPhoto() {
    if (image < 3) {
      image++;
    } else if (image >= 3) {
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

<h1 class="title">Board Design Example 3</h1>

<img src={src[image]} alt="example3 photos" />

<button class="button is-light" on:click={nextPhoto}>Next</button>