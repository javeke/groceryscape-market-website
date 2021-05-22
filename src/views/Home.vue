<template>
  <div class="home">
    <div class="head">
      <div class="text">
        <h3>
          GroceryScape
        </h3>
        <p>
          Remote grocery shopping at your finger tips. <a href="https://groceryscape.web.app">GroceryScape</a> is an online supermarket platform which is designed
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
        <p>
          Here we see where a customer is able to place an order based on recommendations given by the software 
          and is able to browse the store and complete orders. The customer also has the ability to schedule and 
          track orders. 
        </p>
      </div>
      <video controls autoplay muted>
        <source src="../assets/GroceryScape.mp4" type="video/mp4">
        Your browser does not support the video tag.
      </video>
    </div>
    <div  id="demos" class="groceryscape-admin-demo">
      <div>
        <h3>
          GroceryScape Admin allows company owners to manage orders 
        </h3>
        <p>
          Here an administrator is able to monitor and filter all orders by status and is able to
          update the order status so that customers can track orders.
        </p>
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
      font-size: 3em;
      color: green;
    }
    a{
        color: green;
        font-weight: bold;
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
          font-weight: bold;
        }
    }
}

@media screen and (max-width:400px) {
  .about-us-row{
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));

    .text-col{
      order: 1 ;
      padding: 0px 0px;
      h5, h6, p{
        padding-left: 20px;
        padding-right: 20px;
      }
    }
    .image-col{
      order: 2;
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
  h3{
    color: green;
  }
  p{
    padding-left: 20px;
    padding-right: 20px;
  }
  video{
    margin: auto;
    width: 80%;
  }
}

.groceryscape-admin-demo{
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(450px, 1fr));
  align-items: center;
  gap: 10px;
  background: rgb(240, 249, 255);
  padding: 40px;
  h3{
    color: green;
  }
  p{
    padding-left: 20px;
    padding-right: 20px;
  }
  video{
    width: 80%;
    margin: auto;
  }
}

@media screen and (max-width:450px) {
  .groceryscape-demo{
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  }
  .groceryscape-admin-demo{
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  }
}


</style>
