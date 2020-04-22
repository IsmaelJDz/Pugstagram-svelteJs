<script>
  export let nickname;
  export let name;
</script>

<!-- Profile.svelte -->

<style>
  .Profile-content {
    display: flex;
    align-items: center;
  }
  .Profile-avatar img {
    width: 42px;
    height: 42px;
    border-radius: 50%;
  }
  .Profile-info {
    margin: 0 0 0 0.5em;
  }
  .Profile-info h2 {
    font-size: 14px;
    color: black;
    margin: 0;
    padding: 0;
  }
  .Profile-info span {
    font-size: 12px;
    font-weight: normal;
  }

  @media screen and (max-width: 1000px) {
    .Profile {
      display: none;
    }
  }
</style>

<div class="Profile">
  <div class="Profile-content">
    <div class="Profile-avatar">
      <img
        src="https://pbs.twimg.com/profile_images/976652576094437376/Ao8H8lWv_400x400.jpg"
        alt="Logo"
      />
    </div>
    <div class="Profile-info">
      <h2>{ nickname }</h2>
      <span>{ name }</span>
    </div>
  </div>
</div>
