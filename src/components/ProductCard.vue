<script setup>
import { ref } from 'vue'

const props = defineProps(['name', 'category', 'imageUrl', 'ratings', 'discount', 'price'])

const visible = ref(false)
</script>

<template>
  <div class="productContainer">
    <div
      class="productImageContainer"
      v-on:mouseenter="() => (visible = true)"
      v-on:mouseleave="() => (visible = false)"
    >
      <img v-bind:src="props.imageUrl" alt="" />
      <div class="imageIcons" v-if="visible">
        <button class="iconImage">
          <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="100%" viewBox="0 0 48 48">
            <path
              fill="none"
              stroke="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="3"
              d="M15 8C8.925 8 4 12.925 4 19c0 11 13 21 20 23.326C31 40 44 30 44 19c0-6.075-4.925-11-11-11c-3.72 0-7.01 1.847-9 4.674A10.99 10.99 0 0 0 15 8"
            />
          </svg>
        </button>
        <button class="iconImage">
          <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="100%" viewBox="0 0 24 24">
            <path
              fill="currentColor"
              d="M3 3h6v2H6.462l4.843 4.843l-1.415 1.414L5 6.367V9H3zm0 18h6v-2H6.376l4.929-4.928l-1.415-1.414L5 17.548V15H3zm12 0h6v-6h-2v2.524l-4.867-4.866l-1.414 1.414L17.647 19H15zm6-18h-6v2h2.562l-4.843 4.843l1.414 1.414L19 6.39V9h2z"
            />
          </svg>
        </button>
        <button class="iconImage">
          <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="100%" viewBox="0 0 24 24">
            <path
              fill="none"
              stroke="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="1.5"
              d="M16.5 21a1.5 1.5 0 1 0 0-3a1.5 1.5 0 0 0 0 3m-8 0a1.5 1.5 0 1 0 0-3a1.5 1.5 0 0 0 0 3M3.71 5.4h15.214c1.378 0 2.373 1.27 1.995 2.548l-1.654 5.6C19.01 14.408 18.196 15 17.27 15H8.112c-.927 0-1.742-.593-1.996-1.452zm0 0L3 3"
            />
          </svg>
        </button>
      </div>
    </div>
    <div class="detailContainer">
      <div class="categoryRatingsContainer">
        <p>{{ props.category }}</p>
        <div class="ratingContainer">
          <div class="iconContainer">
            <svg xmlns="http://www.w3.org/2000/svg" width="100%" height="100%" viewBox="0 0 24 24">
              <path
                fill="currentColor"
                d="m12 17.275l-4.15 2.5q-.275.175-.575.15t-.525-.2t-.35-.437t-.05-.588l1.1-4.725L3.775 10.8q-.25-.225-.312-.513t.037-.562t.3-.45t.55-.225l4.85-.425l1.875-4.45q.125-.3.388-.45t.537-.15t.537.15t.388.45l1.875 4.45l4.85.425q.35.05.55.225t.3.45t.038.563t-.313.512l-3.675 3.175l1.1 4.725q.075.325-.05.588t-.35.437t-.525.2t-.575-.15z"
              />
            </svg>
          </div>
          <p>{{ props.ratings }}</p>
        </div>
      </div>
      <h3>{{ props.name }}</h3>
      <h4>${{ props.price }} <s v-if="props.discount"></s></h4>
    </div>
  </div>
</template>

<style scoped>
.productContainer {
  width: auto;
  padding: 5px;
  font-family: 'creato display';
}

.productImageContainer {
  position: relative;
  width: 100%;
  /* height: auto; */
  border-radius: 15px;
  overflow: hidden;
}

.productImageContainer img {
  display: block;
  width: 100%;
  object-fit: cover;
  object-position: center;
}

.visible {
  display: block;
}

.invisible {
  display: none;
}

.imageIcons {
  position: absolute;
  right: 15px;
  top: 15px;
}

.iconImage {
  display: flex;
  flex-direction: row;
  width: 40px;
  height: 40px;
  padding: 8px;
  margin-bottom: 5px;
  border: none;
  border-radius: 100%;
  background-color: white;

  cursor: pointer;
}

.iconContainer {
  width: 25px;
  height: fit-content;
  color: #febb2e;
}

.ratingContainer {
  display: flex;
  align-items: center;
  gap: 5px;
}

.categoryRatingsContainer {
  display: flex;
  gap: 0;
  height: fit-content;
  justify-content: space-between;
  align-items: center;
  color: rgb(155, 155, 155);
}

.categoryRatingsContainer p,
h3,
h4 {
  margin: 0;
}

.detailContainer {
  display: flex;
  flex-direction: column;
  gap: 10px;
  margin-top: 15px;
}
</style>
