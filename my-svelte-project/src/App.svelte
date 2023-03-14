<script>
  import svelteLogo from './assets/svelte.svg'
  import Counter from './lib/Counter.svelte'
</script>

<main>
  <header>
    <h1>Monkey Dating</h1>
    <nav>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About Us</a></li>
        <li><a href="#">Contact Us</a></li>
      </ul>
    </nav>
  </header>
  <main>
    <section class="featured">
      <h2>Featured Monkeys</h2>
      <ul>
        <li>
          <img src="https://placehold.it/200x200" alt="Monkey Profile Picture">
          <h3>Monkey Name</h3>
          <p>Age: 5 years</p>
          <p>Location: Jungle</p>
          <a href="#" class="btn">View Profile</a>
        </li>
        <li>
          <img src="https://placehold.it/200x200" alt="Monkey Profile Picture">
          <h3>Monkey Name</h3>
          <p>Age: 6 years</p>
          <p>Location: Rainforest</p>
          <a href="#" class="btn">View Profile</a>
        </li>
        <li>
          <img src="https://placehold.it/200x200" alt="Monkey Profile Picture">
          <h3>Monkey Name</h3>
          <p>Age: 4 years</p>
          <p>Location: Mountain</p>
          <a href="#" class="btn">View Profile</a>
        </li>
      </ul>
    </section>
    <section class="search">
      <h2>Find a Monkey</h2>
      <form>
        <label for="location">Location:</label>
        <input type="text" id="location" name="location" placeholder="Enter location">
        <label for="age">Age:</label>
        <select id="age" name="age">
          <option value="">Select age</option>
          <option value="1">1 year</option>
          <option value="2">2 years</option>
          <option value="3">3 years</option>
          <option value="4">4 years</option>
          <option value="5">5 years</option>
          <option value="6">6 years</option>
          <option value="7">7 years</option>
          <option value="8">8 years</option>
          <option value="9">9 years</option>
          <option value="10+">10+ years</option>
        </select>
        <button type="submit" class="btn">Search</button>
      </form>
    </section>
  </main>
  <footer>
    <p>&copy; 2023 Monkey Dating</p>
  </footer>
</main>

<style>

  nav ul {
  list-style: none;
  }
  .featured ul {
    list-style: none;
  }

</style>
