<script>

  import monke1 from '../assets/Monke_pics/images.jpg'
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
          <img src={monke1} alt="Monkey Profile Picture">
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
  * {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

/* Body styles */
body {
  font-family: Arial, sans-serif;
  font-size: 16px;
  line-height: 1.5;
  background-color: #f2f2f2;
}

/* Main styles */
main {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}

/* Header styles */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}

h1 {
  font-size: 36px;
  font-weight: bold;
  color: #333;
}

nav ul {
  list-style: none;
  display: flex;
}

nav li {
  margin-left: 20px;
}

nav a {
  text-decoration: none;
  color: #333;
  font-weight: bold;
}

/* Featured section styles */
.featured {
  margin-bottom: 40px;
}

.featured h2 {
  font-size: 24px;
  font-weight: bold;
  color: #333;
  margin-bottom: 20px;
}

ul {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  list-style: none;
  margin: 0;
  padding: 0;
}

li {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 10px;
  padding: 20px;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
}

img {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 20px;
}

h3 {
  font-size: 20px;
  font-weight: bold;
  color: #333;
  margin-bottom: 10px;
}

p {
  font-size: 16px;
  color: #777;
  margin-bottom: 10px;
}

.btn {
  display: inline-block;
  padding: 10px 20px;
  background-color: #333;
  color: #fff;
  text-decoration: none;
  border-radius: 5px;
  transition: background-color 0.3s ease;
}

.btn:hover {
  background-color: #555;
}

/* Search section styles */
.search h2 {
  font-size: 24px;
  font-weight: bold;
  color: #333;
  margin-bottom: 20px;
}

form {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  background-color: #fff;
  padding: 20px;
  border-radius: 10px;
  box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
}
      
.featured ul li img {
  display: block;
  margin: 0 auto;
}

/* Styling for the search section */
.search {
  text-align: center;
}

.search h2 {
  font-size: 2rem;
  margin-top: 40px;
}

.search form {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin-top: 20px;
}

.search label {
  font-weight: bold;
  margin-right: 10px;
  display: inline-block;
}

.search input[type="text"],
.search select {
  padding: 10px;
  border-radius: 5px;
  border: none;
  margin-right: 5px;
  margin-bottom: 0px;
  width: 200px;
}

.search button {
  background-color: #00bcd4;
  color: #fff;
  border: none;
  border-radius: 5px;
  padding: 10px 20px;
  text-align: center;
  text-decoration: none;
  transition: background-color 0.3s ease;
  display: inline-block;
}

.search button:hover {
  background-color: #007a8a;
}

</style>
