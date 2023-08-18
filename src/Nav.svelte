<script src="https://kit.fontawesome.com/7010972835.js" crossorigin="anonymous">
  import logo from "./assets/logo_test.png";
</script>

<header>
  <nav>
    <section class="heading">
      <img src={logo} alt="logo" />
      <div class="title">
        <p>iConnect</p>
        <p>Connect Quicker</p>
        <p>Connect Easier</p>
      </div>
    </section>
    <section class="nav-items">
      <span class="material-symbols-outlined"> light_mode </span>
      <button class="contact-s btn-l btn-s">Contact</button>
      <button class="cart-s btn-l btn-s">Cart</button>
    </section>
  </nav>
  <div class="grad" />
</header>

<style>
  @import url("https://fonts.googleapis.com/css2?family=Cabin+Condensed&display=swap");

  /* Layout Styles */

  .title {
    display: flex;
    flex-direction: column;
    margin-left: 0.5vw;
  }

  .heading {
    display: flex;
    align-items: center;
  }

  nav {
    padding: 1% 2%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    font-family: "Cabin Condensed", sans-serif;
  }

  .nav-items {
    display: flex;
    align-items: center;
  }

  span {
    font-size: 3vw;
  }

  .nav-items > * {
    margin-right: 0.6vw;
  }

  .btn-l {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  /* Design CSS */

  .title > p {
    font-size: 1.1rem;
    text-transform: uppercase;
  }

  .btn-s {
    border: none;
    padding: 2vh;
    width: 8vw;
    border-radius: 27px;
    font-family: "Cabin Condensed", sans-serif;
    font-size: 1.2rem;
  }

  .contact-s {
    background-color: #6ee2f5;
    background: linear-gradient(180deg, #6ee2f5 0%, #a96dfc 100%),
      linear-gradient(0deg, #ffffff, #ffffff);
  }

  .cart-s {
    background-color: black;
    color: #6ee2f5;
    border: 3px solid #6ee2f5;
    transition: all 0.5s ease-in-out;
  }

  .cart-s:hover {
    background: #6ee2f5;
    color: black;
    border-color: black;
  }

  .grad {
    background: linear-gradient(-90deg, #8b48df 7.81%, #6ee2f5 56.25%);
    height: 1vh;
  }
</style>
