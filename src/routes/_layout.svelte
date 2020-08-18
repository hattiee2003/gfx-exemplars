<script>
	import Nav from './_components/Nav.svelte'

	export let segment
</script>

<style>
footer{
	height: 100px !important;
}
</style>

<Nav {segment}/>

<main class="section">
	<slot></slot>
</main>

<footer class="footer">
  <div class="content has-text-centered">
    <p>
      <strong>Graphics Exemplars</strong> by Harriet Eglinton. The source code is licensed by
      <a href="http://opensource.org/licenses/mit-license.php" style="color: #3273dc !important;">MIT</a>. The website content is licensed by Rangi Ruru Girls School.
    </p>
  </div>
</footer>
