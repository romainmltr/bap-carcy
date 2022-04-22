<script xmlns="http://www.w3.org/1999/html">
export  default {
  data(){
    return{
      message:""
    }
  }
}

</script>

<template>

          <section class="CardClass">
              <div class="card">
                <div class="card-avatar">
                  <img src="https://www.pngitem.com/pimgs/m/37-370509_the-rock-head-png-dwayne-johnson-transparent-png.png">
                </div>

              <div class="card-details">
              <div class="name">Saitama</div>
              <div class="occupation">Hero</div>

              <div class="card-about">
                    <div class="item">
                        <span class="value">25</span>
                        <span class="label">Age</span>
                    </div>

                    <div class="item">
                        <span class="value">70 kg </span>
                        <span class="label">Weight</span>
                    </div>
              </div>
          </div>

      <div class="skills">
          <span class="value">Immeasurable Physical Prowess, Supernatural Reflexes and Senses, Invulnerability, Indomitable Will, Enhanced Fighting Skill</span>
        </div>
    </div>

</section>


</template>

<style lang="scss">

body {
  background: teal;
  font: 300 18px/18px Roboto
}

section.CardClass{
  margin-top: 75%;
  transform: rotate(-90deg)
}
.card {
  width: 100%;
  border-radius: 0.75rem;
  box-shadow:  0 22px 70px 4px rgba(0,0,0,0.56), 0 0 0 1px rgba(0, 0, 0, 0.3);
  background: black;
  display: grid;
  grid-template-columns: 40% auto;
  color: white;
  align-items: center;
  will-change: transform;
  transition: transform 0.25s cubic-bezier(0.4, 0.0, 0.2, 1), box-shadow 0.25s cubic-bezier(0.4, 0.0, 0.2, 1);
  &:hover {
    transform: scale(1.1);
    box-shadow:  0 32px 80px 14px rgba(0,0,0,0.36), 0 0 0 1px rgba(0, 0, 0, 0.3);
  }
}

.card-details {
  padding: 1rem;
}

.name {
  font-size: 1.25rem;
}

.occupation {
  font-weight: 600;
  color: var(--primary);
}

.card-avatar {
  display: grid;
  place-items: center;
  img{
    width: 80px;
  }
}

svg {
  fill: white;
  width: 65%;
}

.card-about {
  margin-top: 1rem;
  display: grid;
  grid-auto-flow: column;
}

.item {
  display: flex;
  flex-direction: column;
  margin-bottom: 0.5rem;

  .value {
    font-size: 1rem;
  }

  .label {
    margin-top: 0.15rem;
    font-size: 0.75rem;
    font-weight: 600;
    color: var(--primary);
  }
}

.skills {
  display: flex;
  flex-direction: column;
  margin-top: 0.75rem;
  margin-left:20px;
  margin-top: 10px;
  .label {
    font-size: 1rem;
    font-weight: 600;
    color: var(--primary);
  }

  .value {
    margin-top: 0.15rem;
    font-size: 0.75rem;
    line-height: 1.25rem;
  }
}
</style>
