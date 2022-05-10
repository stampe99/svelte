<script>
    import { url } from '@roxi/routify'
</script>

<style>
  .huge {
    font-size: 12rem;
  }
  .e404 {
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
    margin: 10px;
  }
</style>

<div class="e404">
  <div class="huge">404</div>
  <div class="big">Uh oh... We cannot find the page you're searching for... <br>$ {location.href} <br>
  <!-- link to the parent folder of _fallback.svelte -->
  <a href={$url('../')}>Go back</a>
  </div>
</div>
