<script>
  const items = [{ title: "Product-1", quantity: 5, price: 99.8 }];

  let total = 0;
  items.forEach((item) => (total += item.quantity * item.price));
</script>

<main class="cart-l cart-s">
  <section class="cart-body-l cart-body-s">
    <div class="head-l head-s">
      <h2>Cart</h2>
      <button class="close-s close-l">
        <span class="material-symbols-outlined">
            close
            </span>
      </button>
    </div>
    <div class="divider">
      <div class="big" />
    </div>
    <div class="products-l products-s">
      {#each items as item}
        <div class="product-item-l product-item-s">
          <section class="img-l">
            <div class="picture" />
          </section>
          <section class="info-l info-s">
            <h1>{item.title}</h1>
            <section class="numbers-l">
              <div class="quantity-l">
                <label for="quantity">Quantity</label>
                <input type="number" value={item.quantity}/>
              </div>
              <div class="price"><p>AED{item.price}</p></div>
            </section>
          </section>
        </div>
      {/each}
    </div>
  </section>
  <div class="summary-l summary-s">
    <h3>Total</h3>
    <p>AED {total}</p>
  </div>
</main>

<style>
  /* * {
    font-family: "Cabin Condensed", sans-serif;
  } */

  /* Layout Styles */

  .cart-l {
    height: 100vh;
    position: absolute;
    top: 0;
    right: 0;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
  }

  .cart-body-l {
    display: flex;
    flex-direction: column;
    padding: 4% 4%;
    /* justify-content: center; */
  }

  .head-l {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .product-item-l {
    display: flex;
    align-items: center;
    /* justify-content: center; */
    width: 100%;
    /* padding: 0% 10% 1%; */
  }

  .img-l {
    margin-right: 1vw;
  }

  .info-l {
    display: flex;
    flex-direction: column;
    flex: 1;
  }

  .quantity-l {
    display: flex;
    flex-direction: column;
  }

  .numbers-l {
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .summary-l {
    padding: 4% 4%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .divider {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .close-l {
    padding: 0%;
    display: flex;
    align-items: center;
    padding: 1%;
  }

  h1 {
    margin: 0 0 4% 0;
  }

  /* Design Styles */

  h1, h2, h3, p, label, input {
    font-family: 'Cabin Condensed', sans-serif;
  }

  .cart-s {
    border: 1px solid rgb(238, 238, 238);
    width: 30vw;
    background: rgb(255, 255, 255);
  }

  h2 {
    font-size: 3rem;
  }

  .summary-s {
    background-color: rgb(238, 238, 238);
  }

  .summary-s > h3 {
    font-size: 2rem;
  }

  .picture {
    background-color: gray;
    width: 50px;
    height: 50px;
    border-radius: 100%;
  }

  input {
    width: 2vw;
    height: 2vw;
    text-align: center;
  }

  .big {
    height: 0.5vh;
    margin: 2% 0;
    width: 100%;
    background-color: black;
  }

  .close-s {
    border: 2px solid rgb(225, 225, 225);
    border-radius: 100%;
    background-color: white;
    transition: all 300ms ease-in-out;
  }

  .close-s:hover {
    background-color: rgb(225, 225, 225);
  }
</style>
