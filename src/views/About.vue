<template>
  <div class="about">
    <div class="team-section">
        <div class="title">
            <h4><i class="bi bi-people-fill"></i><b>Our Team</b></h4>
            <p> <a href="https://groceryscape.web.app">GroceryScape</a> was built by a group of young and brilliant software developers. They all have their individual 
              strengths and weaknesses and worked tirelessly to complement each other's strength to deliver the project</p>
        </div>
        <div class="team-row">
            <div class="card">
                <div class="card-image">
                    <img src="../assets/malik.jpg">
                </div>
                <div class="card-content">
                    <p>
                      I am a fullstack software developer, who mainly focuses on database design and backend frameworks. 
                      I am a very hardworking individual and a fan of the Spanish football club Real Madrid. 
                    </p>
                    <h6> -Malik Edwards</h6>
                    <p>Database Developer</p>
                    <p class="social-icons">
                      <a href="https://www.instagram.com/realmalz/"><i class="bi bi-instagram"></i></a>
                      <a href="https://www.linkedin.com/in/malik-e-90a754139/"><i class="bi bi-linkedin"></i></a>
                      <a href="https://github.com/malz101"><i class="bi bi-github"></i></a>
                    </p>
                </div>
            </div>
            <div class="card">
                <div class="card-image">
                    <img src="../assets/milton.jpg">
                </div>
                <div class="card-content">
                    <p>
                      I am a very diligent computer scientist with excellent time and project management skills
                      which complements my problem solving skills. I am a quick learner and web development enthusiast.
                    </p>
                    <h6>- Milton Francis</h6>
                    <p>Backend Developer</p>
                    <p class="social-icons">
                      <a href="https://www.linkedin.com/in/milton-francis-66b2471a7/"><i class="bi bi-linkedin"></i></a>
                      <a href="https://github.com/legend19410"><i class="bi bi-github"></i></a>
                    </p>
                </div>
            </div>
            <div class="card">
                <div class="card-image">
                    <img src="../assets/jason.jpg">
                </div>
                <div class="card-content">
                    <p>
                      I am a very meticulous developer who ensures to conduct a deep research into any
                      project that I am working on. My passion lies in computer architecture and low level embedded
                      systems. 
                    </p>
                    <h6>- Jason Hunter</h6>
                    <p>AI Developer</p>
                    <p class="social-icons">
                      <a href="https://www.linkedin.com/in/jason-hunter-363569142"><i class="bi bi-linkedin"></i></a>
                      <a href="https://github.com/jahunter767"><i class="bi bi-github"></i></a>
                    </p>
                </div>
            </div>
            <div class="card">
                <div class="card-image">
                    <img src="../assets/javier.jpg">
                </div>
                <div class="card-content">
                    <p>
                      I am a football lover, math, physics and foreign languange enthusiast. I am determined to be able to speak at least 5 languages fluently by 30. As for career interest, 
                      I am looking to pursue studies in game development, cybersecurity and IOT embedded systems.  
                    </p>
                    <h6>- Javier Bryan</h6>
                    <p>Frontend Developer </p>
                    <p class="social-icons">
                      <a href="https://www.twitter.com/javiii_don"><i class="bi bi-twitter"></i></a>
                      <a href="https://www.instagram.com/javiertjbryan"><i class="bi bi-instagram"></i></a>
                      <a href="https://www.linkedin.com/in/javier-bryan-b06510131/"><i class="bi bi-linkedin"></i></a>
                      <a href="https://www.github.com/javeke"><i class="bi bi-github"></i></a>
                    </p>
                </div>
            </div>
        </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.about{
  background: rgb(240, 249, 255);
}

.title{
  padding: 30px 0;
  h4{
    font-size: 2.5em;
    display: flex;
    justify-content: center;
    gap: 10px ;
  }
  p{
    max-width: 70%;
    margin: auto;
    font-size: 1.1em;
  }
  a{
    color: green;
    font-weight: bold;
  }
}

.team-row{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    background: #00242c;
    .card{
        color: #fff;
        background: #00242c;
        box-shadow: none;
        max-width: 250px;
        padding: 12px;
        box-sizing: content-box;
        text-align: center;
        border: none;
        border-radius: 0;
        .card-image{
            display: flex;
            justify-content: center;
            padding: 20px 0;
            img{
                border-radius: 50%;
                width: 160px;
                height: 160px;
            }
        }
        .social-icons{
          display: flex;
          justify-content: center;
          gap: 10px;
          font-size: 20px;
          a{
            color: #81e291;
          }
          a:hover{
             color: #2c3e50;
          }
        }
    }
}
</style>