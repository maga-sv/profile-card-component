<script setup></script>

<template>
  <div class="card">
    <div class="card__intro">
      <img
        src="@/assets/images/bg-pattern-card.svg"
        alt=""
        class="card__intro-cover"
      />

      <div class="card__intro-ava">
        <img
          src="@/assets/images/image-victor.jpg"
          alt=""
          class="card__intro-ava-img"
        />
      </div>
    </div>

    <div class="card__content">
      <a href="#!" class="card__content-username"
        >Victor Crests <span>26</span></a
      >

      <p class="card__content-userlocation">London</p>

      <div class="card__content-stats"></div>
    </div>

    <div class="card__stats">
      <div class="card__stats-card">
        <span class="card__stats-card-num">80K</span>
        <span class="card__stats-card-name">Followers</span>
      </div>
      <div class="card__stats-card">
        <span class="card__stats-card-num">80K</span>
        <span class="card__stats-card-name">Likes</span>
      </div>
      <div class="card__stats-card">
        <span class="card__stats-card-num">80K</span>
        <span class="card__stats-card-name">Photos</span>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  // min-height: 374px;
  // height: 100%;
  max-width: 354px;
  height: 100%;
  border-radius: 20px;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  align-items: center;
  background: var(--cardColor);
  -moz-user-select: -moz-none;
  -khtml-user-select: none;
  -webkit-user-select: none;
  -o-user-select: none;
  user-select: none;

  &__intro {
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 140px;
    flex-grow: 1;
    position: relative;

    &-cover {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
    &-ava {
      position: absolute;
      bottom: -36%;
      width: 106px;
      height: 106px;
      border-radius: 50%;
      overflow: hidden;
      border: 6px solid #fff;

      &-img {
        width: 100%;
        height: 100%;
      }
    }
  }

  &__content {
    margin-top: 45px;
    padding: 25px 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;

    &-username {
      font-weight: 700;
      font-size: 18px;
      color: var(--secondaryColor);
      margin-bottom: 10px;

      span {
        color: var(--accentColor);
        font-weight: 400;
      }
    }
    &-userlocation {
      color: var(--accentColor);
    }

    border-bottom: 1px solid var(--secAccentColor);
  }

  &__stats {
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    width: 100%;
    padding: 25px 10px;

    &-card {
      display: flex;
      flex-direction: column;
      align-items: center;
      &-num {
        font-weight: 700;
        color: var(--secondaryColor);
        font-size: 18px;
      }
      &-name {
        font-size: 10px;
        letter-spacing: 1px;
        color: var(--secAccentColor);
      }
    }
  }
}
</style>
