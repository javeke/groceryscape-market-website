<template>
  <div class="home">
    <div class="head">
      <div class="text">
        <h3>
          GroceryScape
        </h3>
        <p>
          Remote grocery shopping at your finger tips. GroceryScape is an online supermarket platform which is designed
          to provide one of the best customer experiences and allow the site to make relevent and on point suggestions to
          customer for furture purchases. 
        </p>
      </div>
      <img src="../assets/supermarket1.png" alt="GroceryScape Delivery Man" class="logo">
    </div>

    <div class="about-us-row">
      <div class="image-col">
          <img src="../assets/supermarket.png" alt="Supermarket Image">
      </div>
      <div class="text-col">
          <h5>
              Do more productive shopping with <a href="https://groceryscape.web.app">GroceryScape</a>.
          </h5>
          <h6>How it works</h6>
          <p>
              <a href="https://groceryscape.web.app">GroceryScape</a> is intelligent enough to make purchase history and rating recommendations for customers
              also able to make recommendations based on what items are commonly purchased together to make shopping
              easier and more seamless for consumers. 
          </p>
          <h6>Our Goal</h6>
          <p>
              We aimed to build a complete software solution for both consumers and company ownwers alike. The main <a href="https://groceryscape.web.app">GroceryScape</a>
              application frontend would allow consumers to make market purchases, schedule delivery and view order status while 
              the administrative dashboard of the application would allow company owners to view all orders and the assign
              relevent personnel to handle the delivery of the items ordered and while being able to update the status for
              the orders so the customers can track their orders.
          </p>
      </div>
    </div>
    <div class="groceryscape-demo">
      <div>
        <h3>
          Take a look at the demo of GroceryScape
        </h3>
      </div>
      <video controls autoplay muted>
        <source src="../assets/GroceryScape.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
    </div>
    <div class="groceryscape-admin-demo">
      <div>
        <h3>
          GroceryScape Admin allows company owners to manage orders 
        </h3>
      </div>
      <video controls autoplay muted>
        <source src="../assets/GroceryScape-Admin.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
}
</script>

<style lang="scss" scoped>
.head{
  display:  grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
  background: rgb(240, 249, 255);
  .text{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    padding: 30px;
    gap: 20px;
    h3{
      font-size: 4em;
      color: green;
    }
    p{
      font-size: 1.5em;
    }
  }
  img{
    padding-top: 40px;
    text-align: center;
    width: 100%;
  }

}


.about-us-row{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
    gap: 10px;
    background: rgb(240, 249, 255);
    .image-col{
        border-radius: 10px;
        img{
            max-width: 100%;
            object-fit: contain;
        }
    }
    .text-col{
        padding: 0px 24px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        h5{
            font-weight: bold;
            color: green;
            margin-bottom: 32px;
        }

        h6{
            font-weight: bold;
            font-size: 1.5em;
            color: green;
        }
        p{
            margin-bottom: 32px;
            font-size: 1.1em;
        }
        a{
          color: green;
        }
    }
}

.groceryscape-demo{
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
  gap: 10px;
  background: rgb(240, 249, 255);
  padding: 40px;
  align-items: center;
  video{
    width: 100%;
  }
}

.groceryscape-admin-demo{
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
  align-items: center;
  gap: 10px;
  background: rgb(240, 249, 255);
  padding: 40px;
  video{
    width: 100%;
  }
}


</style>
