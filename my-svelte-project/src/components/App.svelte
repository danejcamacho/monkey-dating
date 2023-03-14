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
  body {
        font-family: Arial, sans-serif;
        margin: 0;
        padding: 0;
      }
      
      /* Header styles */
      header {
        background-color: #00bcd4;
        color: #fff;
        display: flex;
        justify-content: space-between;
        padding: 20px;
      }
      
      h1 {
        margin: 0;
      }
      
      nav ul {
        list-style: none;
        margin: 0;
        padding: 0;
        display: flex;
      }
      
      nav li {
        margin: 0 10px;
      }
      
      nav li a {
        color: #fff;
        text-decoration: none;
        font-weight: bold;
      }
      
      /* Featured section styles */
      .featured {
        display: flex;
        justify-content: space-around;
        align-items: center;
        flex-wrap: wrap;
        padding: 50px 0;
      }
      
      .featured li {
        background-color: #f2f2f2;
        margin: 20px;
        padding: 20px;
        text-align: center;
        border-radius: 5px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
      }
      
      .featured li img {
        border-radius: 50%;
        margin-bottom: 20px;
      }
      
      .featured li h3 {
        margin: 0;
      }
      
      .featured li p {
        margin: 0;
        font-size: 14px;
        color: #888;
      }
      
      .featured li .btn {
        display: block;
        margin-top: 20px;
        background-color: #00bcd4;
        color: #fff;
        padding: 10px 20px;
        text-align: center;
        text-decoration: none;
        border-radius: 5px;
        transition: background-color 0.3s ease;
      }
      
      .featured li .btn:hover {
        background-color: #007a8a;
      }
      
      /* Search section styles */
      .search {
        background-color: #eee;
        padding: 50px;
        text-align: center;
      }
      
      .search h2 {
        margin-top: 0;
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
      }
      
      .search input[type="text"],
      .search select {
        padding: 10px;
        border-radius: 5px;
        border: none;
        margin-right: 10px;
        margin-bottom: 10px;
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
      }
      
      .search button:hover {
        background-color: #007a8a;
      }

</style>
