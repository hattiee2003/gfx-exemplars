<script>
  let src = [
    "/img/board/board_exemplar_1_1.jpeg",
    "/img/board/board_exemplar_1_2.jpeg",
    "/img/board/board_exemplar_1_3.jpeg",
    "/img/board/board_exemplar_1_4.jpeg",
    "/img/board/board_exemplar_1_5.jpeg",
    "/img/board/board_exemplar_1_6.jpeg"
  ];

  let image = 0;

  function nextPhoto() {
    if (image < 5) {
      image++;
    } else if (image >= 5) {
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

<h1 class="title">Board Design Example 1</h1>

<img src={src[image]} alt="example1 photos" />

<button class="button is-light" on:click={nextPhoto}>Next</button>