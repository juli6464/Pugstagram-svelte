<script>
    export let nickname;
    export let name;
</script>

<style>
    .Profile-content {
      display: flex;
      align-items: center;
      padding-top: 73px;
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
  

<div class="Profile">
    <div class="Profile-content">
        <div class=Profile-avatar>
            <img src="https://lh3.googleusercontent.com/ogw/ADea4I7SHv2HQLOAOegPY7UHgjEoehB06XCr89JhYeb1C60=s32-c-mo" alt="">
        </div>
        <div class="Profile-info">
            <h2>{nickname}</h2>
            <span>{name}</span>
        </div>
    </div>
</div>