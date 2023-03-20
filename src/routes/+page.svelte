<script>  
    let list = [
      {
        name: "Justin",
        pic: "/Justin.jpg",
        age: 6,
        location: "Rainforest",
        bio: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec molestie suscipit ex, sed mollis dolor. Phasellus euismod est ut purus tempus lobortis. Ut ullamcorper orci eget tortor dapibus iaculis. Maecenas eu condimentum nisi. Quisque consequat venenatis sodales. Duis eu fringilla sem, ac bibendum urna. Nunc gravida metus sed cursus aliquet. Nullam ac lectus ut nulla aliquet porttitor. Sed nunc justo, bibendum sed hendrerit non, porta sodales velit. Ut mattis ante quis nisi vulputate pellentesque. Aliquam dui nunc, gravida a lacus ac, accumsan sodales mauris. Pellentesque eros felis, molestie nec tellus id, aliquet sodales nunc. Duis velit libero, mattis eget finibus eget, ullamcorper et nunc. Suspendisse semper nibh ac leo efficitur, congue posuere ipsum iaculis. Nulla blandit fringilla sagittis. "
      },
      {
        name: "Charlie",
        pic: "/Charlie.jpg",
        age: 5,
        location: "Jungle",
        bio: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec molestie suscipit ex, sed mollis dolor. Phasellus euismod est ut purus tempus lobortis. Ut ullamcorper orci eget tortor dapibus iaculis. Maecenas eu condimentum nisi. Quisque consequat venenatis sodales. Duis eu fringilla sem, ac bibendum urna. Nunc gravida metus sed cursus aliquet. Nullam ac lectus ut nulla aliquet porttitor. Sed nunc justo, bibendum sed hendrerit non, porta sodales velit. Ut mattis ante quis nisi vulputate pellentesque. Aliquam dui nunc, gravida a lacus ac, accumsan sodales mauris. Pellentesque eros felis, molestie nec tellus id, aliquet sodales nunc. Duis velit libero, mattis eget finibus eget, ullamcorper et nunc. Suspendisse semper nibh ac leo efficitur, congue posuere ipsum iaculis. Nulla blandit fringilla sagittis. "
      },
      {
        name: "Karni",
        pic: "/Karni.jpg",
        age: 4,
        location: "Mountain",
        bio: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec molestie suscipit ex, sed mollis dolor. Phasellus euismod est ut purus tempus lobortis. Ut ullamcorper orci eget tortor dapibus iaculis. Maecenas eu condimentum nisi. Quisque consequat venenatis sodales. Duis eu fringilla sem, ac bibendum urna. Nunc gravida metus sed cursus aliquet. Nullam ac lectus ut nulla aliquet porttitor. Sed nunc justo, bibendum sed hendrerit non, porta sodales velit. Ut mattis ante quis nisi vulputate pellentesque. Aliquam dui nunc, gravida a lacus ac, accumsan sodales mauris. Pellentesque eros felis, molestie nec tellus id, aliquet sodales nunc. Duis velit libero, mattis eget finibus eget, ullamcorper et nunc. Suspendisse semper nibh ac leo efficitur, congue posuere ipsum iaculis. Nulla blandit fringilla sagittis. "
      },
      {
        name: "Aaron",
        pic: "/Aaron.jpg",
        age: 4,
        location: "Rainforest",
        bio: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec molestie suscipit ex, sed mollis dolor. Phasellus euismod est ut purus tempus lobortis. Ut ullamcorper orci eget tortor dapibus iaculis. Maecenas eu condimentum nisi. Quisque consequat venenatis sodales. Duis eu fringilla sem, ac bibendum urna. Nunc gravida metus sed cursus aliquet. Nullam ac lectus ut nulla aliquet porttitor. Sed nunc justo, bibendum sed hendrerit non, porta sodales velit. Ut mattis ante quis nisi vulputate pellentesque. Aliquam dui nunc, gravida a lacus ac, accumsan sodales mauris. Pellentesque eros felis, molestie nec tellus id, aliquet sodales nunc. Duis velit libero, mattis eget finibus eget, ullamcorper et nunc. Suspendisse semper nibh ac leo efficitur, congue posuere ipsum iaculis. Nulla blandit fringilla sagittis. "
      }

    ]

   

    let name = "";
    let pic = "/noProfilePic.jpg"
    let age = "";
    let location = "";
  

    function addMonkey(){
      list.push({
        name: name,
        pic: pic,
        age: age,
        location: location
      })
      list = list;
    };


</script>
  
  

  <header>
  <a href="/"><img class = "logo" src = "/logo.jpg" href="/" alt = logo/></a>
    <h1>Monkey Dating</h1>
    <nav>
      <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/about">About Us</a></li>
        <li><a href="/contact">Contact Us</a></li>
      </ul>
    </nav>
  </header>


  <main>
    <section class="featured">
      <h2>Featured Monkeys</h2>
      <ul>
        
        {#each list as item}
        <li>
          
          <img src= {item.pic} alt="Monkey Profile">
          <h3>{item.name}</h3>
          <p>Age: {item.age} years</p>
          <p>Location: {item.location}</p>
          <a href="/profiles/{item.name}" class="btn">View Profile</a>
        
        </li>
        {/each}

      </ul>
    </section>

    <section class="add">
      <h2>Add a Monkey</h2>
      <form>
        <label for= "name">Name: <input bind:value = {name} type="text" placeholder="Enter name"></label>
        
        <label for= "pic">Profile Pic: <input type="file"/>  </label>
        
        <label for= "age">Age: <input  bind:value = {age} type= "text" placeholder="Enter age"/></label>
        
        <label for= "location">Location: <input  bind:value = {location} type= "text" placeholder="Enter location"/></label> 

        <button on:click = {addMonkey} type="submit" class="btn">Submit</button>
        
      </form>


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
    <p>&copy; 2023 Monkey Dating Inc. All rights reserved.</p>
  </footer>

  
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
  
  label {
    padding: 10px;
  }
  
  .add form{
    display: flex;
    align-items: center;
  }

  /* Main styles */
  main {
    max-width: 900px;
    margin: 0 auto;
    padding: 20px;
    font-family:   Arial, sans-serif;
  }

  footer {
    max-width: 900px;
    margin: 0 auto;
    padding: 20px;
    font-family:   Arial, sans-serif;
  }
  
  /* Header styles */
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
    max-width: 900px;
    margin: 0 auto;
    padding: 20px;
    font-family:   Arial, sans-serif;
  }
  a:link { text-decoration: none; }
  a:visited { text-decoration: none; }
  a:hover { text-decoration: none; }
  a:active { text-decoration: none; }
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
    font-size: 28px;
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
  h2 {
    font-size: 24px;
    font-weight: bold;
    color: #333;
    margin-bottom: 20px;
    justify-content: center;
    font-size: 2rem;
    margin-top: 40px;
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
  
  
  
  
  form {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin-top: 20px;
  }
  
  label {
    font-weight: bold;
    margin-right: 10px;
    display: inline-block;
  }
  
  input[type="text"],
  select {
    padding: 10px;
    border-radius: 5px;
    border: none;
    margin-right: 5px;
    margin-bottom: 0px;
    width: 200px;
  }
  
  .search button {
    background-color: #505353;
    color: #fff;
    border: none;
    border-radius: 5px;
    padding: 10px 20px;
    text-align: center;
    text-decoration: none;
    transition: background-color 0.3s ease;
    display: inline-block;
  }


  .add button {
    background-color: #505353;
    color: #fff;
    border: none;
    border-radius: 5px;
    padding: 10px 20px;
    text-align: center;
    text-decoration: none;
    transition: background-color 0.3s ease;
    display: inline-block;
  }

  .add button:hover {
    background-color: #0da2b6;
  }
  
  .search button:hover {
    background-color: #0da2b6;
  }
  .logo{
    width: 100px;
    height: 100px;
    
  }
  </style>
  