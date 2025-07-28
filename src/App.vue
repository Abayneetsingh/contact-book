<template>
  <div class="outer-wrapper">
    <div class="app-box">
      <header class="app-header">
        <h1>📒 Contact Book</h1>
        <nav class="nav-links">
          <router-link to="/" exact-active-class="active">Home</router-link>
          <router-link to="/add" exact-active-class="active">Add Contact</router-link>
        </nav>
      </header>

      <main class="app-main">
        <router-view />
      </main>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style scoped>
/* Centering container */
.outer-wrapper {
  display: flex;
  justify-content: center;
  align-items: start;
  padding: 40px;
  background-color: #f0f0f0;
  min-height: 100vh;
}

/* Yellow box */
.app-box {
  background-color: #fff9c4; /* soft yellow */
  border: 2px solid #fbc02d;
  border-radius: 12px;
  padding: 2rem;
  width: 100%;
  max-width: 800px;
  box-shadow: 0 8px 16px rgba(0,0,0,0.1);
}

/* Header */
.app-header {
  text-align: center;
  margin-bottom: 1.5rem;
}

.app-header h1 {
  font-size: 2rem;
  color: #333;
}

/* Nav links */
.nav-links {
  margin-top: 0.5rem;
}

.nav-links a {
  margin: 0 1rem;
  text-decoration: none;
  color: #d17f00;
  font-weight: bold;
  transition: color 0.3s;
}

.nav-links a:hover {
  color: #ff6f00;
  text-decoration: underline;
}

.active {
  border-bottom: 2px solid #ff9800;
}

/* Main content */
.app-main {
  margin-top: 1.5rem;
}
</style>
