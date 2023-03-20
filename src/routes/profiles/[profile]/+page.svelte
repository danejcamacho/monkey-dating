<script>
    import Image from "./Image.svelte"
    
    import { page } from '$app/stores'
    let string = $page.params.profile
    let lower = string.toLowerCase()
    const profile = string.charAt(0).toUpperCase() + lower.slice(1)

	  
    

</script>
<main>
    <header>
        <a href ="/"><img class = "logo" src = "/logo.jpg" alt = logo/></a>
        <a href ="/"><h1>Monkey Dating</h1></a>
      <nav>
        <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/about">About Us</a></li>
          <li><a href="/contact">Contact Us</a></li>
        </ul>
      </nav>
    </header>

    <h1> { profile }'s Page </h1>

    <Image src= "/{profile}.jpg"/>
    
    <img src="/{profile}.jpg" alt=""/>
    
    <br>
    <h2>{profile} likes ...</h2>
    <p>"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec molestie suscipit ex, sed mollis dolor. Phasellus euismod est ut purus tempus lobortis. Ut ullamcorper orci eget tortor dapibus iaculis. Maecenas eu condimentum nisi. Quisque consequat venenatis sodales. Duis eu fringilla sem, ac bibendum urna. Nunc gravida metus sed cursus aliquet. Nullam ac lectus ut nulla aliquet porttitor. Sed nunc justo, bibendum sed hendrerit non, porta sodales velit. Ut mattis ante quis nisi vulputate pellentesque. Aliquam dui nunc, gravida a lacus ac, accumsan sodales mauris. Pellentesque eros felis, molestie nec tellus id, aliquet sodales nunc. Duis velit libero, mattis eget finibus eget, ullamcorper et nunc. Suspendisse semper nibh ac leo efficitur, congue posuere ipsum iaculis. Nulla blandit fringilla sagittis. "</p>
    <br>
    <h2>{profile} dislikes ...</h2>
    <p>"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec molestie suscipit ex, sed mollis dolor. Phasellus euismod est ut purus tempus lobortis. Ut ullamcorper orci eget tortor dapibus iaculis. Maecenas eu condimentum nisi. Quisque consequat venenatis sodales. Duis eu fringilla sem, ac bibendum urna. Nunc gravida metus sed cursus aliquet. Nullam ac lectus ut nulla aliquet porttitor. Sed nunc justo, bibendum sed hendrerit non, porta sodales velit. Ut mattis ante quis nisi vulputate pellentesque. Aliquam dui nunc, gravida a lacus ac, accumsan sodales mauris. Pellentesque eros felis, molestie nec tellus id, aliquet sodales nunc. Duis velit libero, mattis eget finibus eget, ullamcorper et nunc. Suspendisse semper nibh ac leo efficitur, congue posuere ipsum iaculis. Nulla blandit fringilla sagittis. "</p>
    <br>
    <h2>Hobbies</h2>
    <ul>
      <li>Lorem Impsum</li>
      <li>Lorem Impsum</li>
      <li>Banana</li>
    </ul>
</main>





<style>
    
    nav ul {
    list-style: none;
    }
    
    * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
  
  
  
  /* Main styles */
  main {
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
  
  ul {
    padding: 10px;
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
  
  
</style>