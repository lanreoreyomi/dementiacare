<template>
  <div id="container">
    <div class="services" data-aos="fade-up"
         data-aos-duration="2000">
      <div class="services_info">
        <div class="services_img">
          <img src="../assets/Images/consultation.jpeg" alt="consultation">
        </div>
        <div class="services_text">
          <h2>Dementia Consultation</h2>
          <hr>
          <p>
            Our Dementia consultation service is one of the ways we can help a person with a diagnosis of dementia, their career or loved one</p>
          <div class="services_btn">
            <Button type="button" class="btn1">
              <router-link :to="{name: 'Consultation'}" class="router-link" exact v-scroll-to="'#book'">Read More
              </router-link>
            </Button>
          </div>
        </div>
      </div>
      <div class="services_info">
        <div class="services_img">
          <img src="../assets/Images/consultation2.jpeg" alt="nurse">
        </div>
        <div class="services_text">
          <h2> Staffing and Recruitment</h2>
          <hr>
          <p>
            Are you an organization looking for quality care for your facilities? Or an individual looking for quality care at home?
          </p>
          <div class="services_btn">
            <Button type="button" class="btn1">
              <router-link :to="{name: 'Staffing'}" class="router-link" exact v-scroll-to="'#book'">Read More
              </router-link>

            </Button>

          </div>
        </div>
      </div>
      <div class="services_info">
        <div class="services_img">
          <img src="../assets/Images/homecare.jpeg" alt="homecare">
        </div>
        <div class="services_text">
          <h2>Home Care Services</h2>
          <hr>
          <p>
            Getting help at home does not take away your independence, it rather maximize your independence and allows you to continue living at home safely          </p>
          <div class="services_btn">
            <Button type="button" class="btn1">
              <router-link :to="{name: 'Homeservice'}" class="router-link" exact v-scroll-to="'#book'">Read More
              </router-link>

            </Button>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>

export default {
  name: "team"
}
</script>

<style scoped lang="scss">
@import "./src/assets/Colors/colors";
@import "./src/assets/Fonts/fonts";
@import "./src/assets/Buttons/buttons";
@import url('https://fonts.googleapis.com/css2?family=Rozha+One&display=swap');

#container {
  .services {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-gap: 20px;
    color: $textColor;
    margin: 0 auto;
    width: 90%;
    text-align: center;

    .services_info {
      transition: 0.5s;
      width: 90%;
      margin: 0 auto;
      border-top-left-radius: 75px;
      border-bottom-right-radius: 75px;

      color: $headerColor;
      box-shadow: 0 5px 10px rgba(154, 160, 185, .05), 0 15px 40px rgba(166, 173, 201, .2);

      .services_img {
        text-align: center;

        img {
          border-top-left-radius: 65px;
          max-width: 100%;

        }
      }

      .services_text {
        padding: 20px;
        text-align: start;

        h2 {
          font-size: 30px;
          text-align: start;

          &::selection {
            background: $secondaryColor;
          }
        }

        hr {
          margin-bottom: 30px;
        }

        p {
          line-height: 30px;
          margin: 10px auto 10px;

          &::selection {
            background: $secondaryColor;
          }
        }

        .services_btn {
          text-align: center;

          .btn1 {
            @include homeButton;
            background: none;
            color: $headerColor;
            padding: 8px;
            border: 1px solid $highlight;
            width: 140px;
            transition: 0.5s;
            position: relative;
            text-align: center;

            text-decoration: none !important;
            a{
              color: $headerColor;
              text-decoration: none;
            }
            &:hover {
              background: $secondaryColor;
              color: $headerColor;


              img {
                display: block;

              }

            }

            &:before {

            }

          }
        }
      }
    }
  }
}

@media (max-width: 480px) and (-webkit-min-device-pixel-ratio: 2) {
  #container {
    margin-top: 0;

    .services {
      grid-template-columns: 1fr;
      grid-gap: 0;
      width: 100%;

      .services_info {
        margin: 20px auto;

        .services_text {

        }
      }
    }
  }

}



@media(min-width: 411px) and(max-width: 823px) and (-webkit-min-device-pixel-ratio: 2) {
  #container {
    #container {
      margin-top: 0;

      .services {
        grid-template-columns: 1fr;
        grid-gap: 0;
        width: 100%;

        .services_info {
          margin: 20px auto;

          .services_text {

          }
        }
      }
    }
  }
}

@media (max-width: 767px) and (-webkit-min-device-pixel-ratio: 2) {

  #container {
    margin-top: 0;

    .services {
      grid-template-columns: 1fr;
      grid-gap: 0;
      width: 100%;

      .services_info {
        margin: 20px auto;

        .services_text {
h2{
  font-size:20px;
}
        }
      }
    }
  }
}

@media (min-width: 768px) and (max-width: 1024px) and (-webkit-min-device-pixel-ratio: 2) {
  #container {
    margin-top: 0;

    .services {
      grid-template-columns: 1fr;
      grid-gap: 0;
      width: 100%;

      .services_info {
        margin: 20px auto;

        .services_text {

        }
      }
    }
  }
}
</style>