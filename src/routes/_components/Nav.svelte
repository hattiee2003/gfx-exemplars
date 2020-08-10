<script>
  export let segment;
</script>

<style>
  .navbar{
    background-color: #81B29A;
    height: 70px;
  }

  h1{
    font-size: 30px;
    line-height: 70px;
    margin-left: 30px;
    margin-right: 30px;
  }

  .navbar-brand:hover{
    background-color: #F4F1DE !important;
    color: black !important;
  }

  #spacial:hover, #product:hover, #board:hover{
    background-color: #F4F1DE !important;
    color: black !important;
  }

 
</style>

<nav class="navbar">
<h1>Level 1 Graphics Exemplars</h1>
  <div class="navbar-brand">
    <a class="navbar-item" class:is-active={segment === undefined} href=".">
      home
    </a>
  </div>

  <div class="navbar-menu">
    <div class="navbar-start">
      <div class="navbar-item has-dropdown is-hoverable">
        <a href="/spacial/spacial" id="spacial" class="navbar-link">spacial</a>

        <div class="navbar-dropdown">
          <a href="/spacial/spacial.1" class="navbar-item">example 1</a>
          <a href="/spacial/spacial.2" class="navbar-item">example 2</a>
          <a href="/spacial/spacial.3" class="navbar-item">example 3</a>

        </div>
      </div>

      <div class="navbar-menu">
        <div class="navbar-start">
          <div class="navbar-item has-dropdown is-hoverable">
            <a href="/product/product" id="product" class="navbar-link">product</a>

            <div class="navbar-dropdown">
              <a href="/product/product.1" class="navbar-item">example 1</a>
              <a href="/product/product.2" class="navbar-item">example 2</a>
              <a href="/product/product.3" class="navbar-item">example 3</a>
            </div>
          </div>

          <div class="navbar-menu">
            <div class="navbar-start">
              <div class="navbar-item has-dropdown is-hoverable">
                <a href="/board/board" id="board" class="navbar-link">board</a>

                <div class="navbar-dropdown">
                  <a href="/board/board.1" class="navbar-item">example 1</a>
                  <a href="/board/board.2" class="navbar-item">example 2</a>
                  <a href="/board/board.3" class="navbar-item">example 3</a>
                </div>
              </div>

            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</nav>


