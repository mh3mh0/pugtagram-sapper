<script>
  export let nickname;
  export let name;
</script>

<div class="Profile">
  <div class="Profile-content">
    <div class="Profile-avatar">
      <img
        src="https://lh3.googleusercontent.com/VM5g669C0Fpp8PrTnbaAZL3M-02T9rK89JrKL4MKNyAFN_Xs3vOpPFjq2H1rwn8OZ18MsEnCKKFs6j2YH2vivpeF34s_-nLJXx_4DtIZ5qFVXxbuSSmiacjs5IRCbHvch83WIcrz3g=w2400"
        alt=""
      />
    </div>
    <div class="Profile-info">
      <h2>{nickname}</h2>
      <span>{name}</span>
    </div>
  </div>
</div>

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
</style>
