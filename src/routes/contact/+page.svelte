<main>
<header>
    <img class = "logo" src = "/logo.jpg" alt = logo/>
    <h1>Monkey Dating</h1>
    <nav>
      <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/about">About Us</a></li>
        <li><a href="/contact">Contact Us</a></li>
      </ul>
    </nav>
  </header>

<h1>Contact Us!</h1>

<ul>
    <li><h3>David</h3>
        <img src="/gorilla.jpg" alt = monke/>
        <h3>Method of Contact:</h3>
        <p>Bang stick on rock</p>
    </li>
    <li><h3>Dane</h3>
        <img src="/gorilla.jpg" alt = monke/>
        <h3>Method of Contact:</h3>
        <p>Bang rock on stick;<br> wait for smoke signal</p>
    </li>
    <li><h3>Chris</h3>
        <img src="/gorilla.jpg" alt = monke/>
        <h3>Method of Contact:</h3>
        <p>Email: chrispenavelez@gmail.com</p>
    </li>
</ul>


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
  

  
  /* Main styles */
  main {
    max-width: 800px;
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
  .logo{
    width: 100px;
    height: 100px;
    
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