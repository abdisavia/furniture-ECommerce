<script setup></script>

<template>
  <nav>
    <img src="/Logo/Logo_cropped.png" alt="Furniture Logo" width="200px" />
    <div class="nav-links">
      <a href="#" class="nav-link">Home</a>
      <a href="#" class="nav-link">Shop</a>
      <a href="#" class="nav-link">Category</a>
      <a href="#" class="nav-link">About Us</a>
      <a href="#" class="nav-link">Contact Us</a>
      <a href="#" class="nav-link">Blog</a>
    </div>
    <div class="nav-icons">
      <a href="" class="nav-icon">
        <svg xmlns="http://www.w3.org/2000/svg" width="fill" height="fill" viewBox="0 0 24 24">
          <path
            fill="none"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="1.5"
            d="M19 11.5a7.5 7.5 0 1 1-15 0a7.5 7.5 0 0 1 15 0m-2.107 5.42l3.08 3.08"
          />
        </svg>
      </a>
    </div>
  </nav>
</template>

<style scoped>
nav {
  padding: 10px 100px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 70px;
  border: 1px solid black;
}

/* nav-link */
.nav-links {
  width: 100%;
  display: flex;
  gap: 20px;
  justify-content: center;
}

.nav-link {
  font-family: 'creato display';
  text-decoration: none;
  color: #212121;
  font-weight: 500;
}

.nav-icons {
  width: 200px;
  display: flex;
}

.nav-icon {
  color: #212121;
  width: 30px;
  height: 30px;
}
</style>
