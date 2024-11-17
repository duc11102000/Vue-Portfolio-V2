<template>
  <div class="footer">
    <footer>
      <nav>
        <div class="nav-links-container">
          <ul class="nav-links">
            <li><a href="#about">About</a></li>
            <li><a href="#experience">Experience</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
          </ul>
        </div>
      </nav>
      <p class="uppercase">2024 Vue.JS still da best framework !!!!!</p>
    </footer>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.footer {
  position: relative;
}

footer {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  padding: 2rem 0;
  background: #002f4b;
}

nav {
  display: flex;
  justify-content: space-around;
  align-items: center;
}

a {
  color: #fff;
  text-decoration: none;
  text-decoration-color: white;
  transition: all 300ms ease;

  &:hover {
    color: #3f9dd5;
    text-decoration: underline;
    text-underline-offset: 1rem;
    text-decoration-color: #3f9dd5;
  }
}

.nav-links {
  display: flex;
  gap: 2rem;
  list-style: none;
  font-size: 1.5rem;
}

footer p {
  text-align: center;
  color: #fff;
  /* margin-bottom: 20px; */
}
</style>
