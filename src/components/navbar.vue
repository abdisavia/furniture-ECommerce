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
      <a href="" class="nav-icon">
        <svg xmlns="http://www.w3.org/2000/svg" width="fill" height="fill" viewBox="0 0 48 48">
          <path
            fill="none"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="3"
            d="M15 8C8.925 8 4 12.925 4 19c0 11 13 21 20 23.326C31 40 44 30 44 19c0-6.075-4.925-11-11-11c-3.72 0-7.01 1.847-9 4.674A10.99 10.99 0 0 0 15 8"
          />
        </svg>
      </a>
      <a href="" class="nav-icon">
        <svg xmlns="http://www.w3.org/2000/svg" width="fill" height="fill" viewBox="0 0 24 24">
          <path
            fill="none"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="1.5"
            d="M16.5 21a1.5 1.5 0 1 0 0-3a1.5 1.5 0 0 0 0 3m-8 0a1.5 1.5 0 1 0 0-3a1.5 1.5 0 0 0 0 3M3.71 5.4h15.214c1.378 0 2.373 1.27 1.995 2.548l-1.654 5.6C19.01 14.408 18.196 15 17.27 15H8.112c-.927 0-1.742-.593-1.996-1.452zm0 0L3 3"
          />
        </svg>
      </a>
      <a href="" class="nav-icon">
        <svg xmlns="http://www.w3.org/2000/svg" width="fill" height="fill" viewBox="0 0 24 24">
          <path
            fill="none"
            stroke="currentColor"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="1.5"
            d="M19.618 21.25c0-3.602-4.016-6.53-7.618-6.53s-7.618 2.928-7.618 6.53M12 11.456a4.353 4.353 0 1 0 0-8.706a4.353 4.353 0 0 0 0 8.706"
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
  justify-content: end;
  gap: 30px;
}

.nav-icon {
  color: #212121;
  width: 30px;
  height: 30px;
}
</style>
