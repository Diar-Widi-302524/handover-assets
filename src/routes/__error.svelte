<script context="module">
  export function load({ error }) {
    return {
      props: { message: error.message },
    };
  }
</script>

<script>
  //export let message;
</script>

<div class="error">
  <h2>Ooops</h2>
  <p>I'm sorry your page doesn't exist</p>
  <a href="/guides">Back to Guides</a>
</div>

<style>
  .error {
    text-align: center;
    margin-bottom: 60px;
  }
</style>
