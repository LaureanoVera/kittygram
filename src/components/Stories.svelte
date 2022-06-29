<script>
  export let nickname;
  // export let name;
</script>

<article class="Stories">
  <div class="Stories-container">
    <div class="Stories-head">
      <h2>Historias</h2>
      <span>Ver todas</span>
    </div>
    <div class="Stories-items">
      <div class="Stories-item">
        <div class="Stories-item-box">
          <img
            src="https://avatars.githubusercontent.com/u/77276651?s=400&u=d222499cf5cff08a206d3d78649a02a546c0d828&v=4"
            alt="Imagen de perfil"
          />
        </div>
        <h2>
          {nickname}
          <span>17 horas</span>
        </h2>
      </div>
    </div>
  </div>
</article>

<style>
  .Stories {
    border: 1px solid rgba(219, 219, 219, 1);
    border-radius: 4px;
    margin: 1em 0;
    padding: 0.5em 1em;
    background-color: white;
  }
  .Stories-item img {
    width: 32px;
    height: 32px;
    border-radius: 50%;
  }
  .Stories-item {
    display: flex;
    align-items: center;
    margin: 0 0 0.5em 0;
  }
  .Stories-item h2 {
    font-size: 14px;
    color: black;
    margin: 0 0 0 0.5em;
  }
  .Stories-item h2 span {
    display: block;
    font-size: 9px;
    text-transform: uppercase;
    color: gray;
  }
  .Stories-head {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0.5em 0 0 0;
  }
  .Stories-head h2 {
    font-size: 12px;
    font-weight: 600;
  }
  .Stories-head span {
    font-size: 12px;
    font-weight: normal;
    color: black;
  }
  .Stories-items {
    margin: 0.5em 0 0.5em 0;
  }
  .Stories-item-box {
    width: 32px;
    height: 32px;
    border: double 2px transparent;
    border-radius: 100%;
    background-image: linear-gradient(#fff, #fff),
      radial-gradient(circle at top left, #f09433, #bc1888);
    background-origin: border-box;
    background-clip: content-box, border-box;
  }
</style>
