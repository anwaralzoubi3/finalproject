# finalproject
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>

  <title>Full Responsive Web Page</title>

  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/css/bootstrap.min.css" rel="stylesheet">

  <!-- Font Awesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">

  <style>

*{
  margin:0;
  padding:0;
  box-sizing:border-box;
}

/* FIXED SMOOTH SCROLL */

html{
  scroll-behavior:smooth;
}

body{
  font-family:Arial, Helvetica, sans-serif;
  background:#f3f3f3;

  overflow-x:hidden;
  overflow-y:auto;

  -webkit-overflow-scrolling:touch;
}

/* CAROUSEL */

.carousel,
.carousel-inner,
.carousel-item{
  width:100%;
  min-height:100vh;
}

/* SMOOTH MOBILE SWIPE */

.carousel{
  touch-action:pan-y;
}

.carousel-item{
  transition:transform .6s ease-in-out;
}

/* MAIN PAGE */

.main-page{
  width:100%;
  min-height:100vh;
  display:flex;
  flex-wrap:wrap;
}

/* LEFT SECTION */

.left-side{
  flex:1;
  min-width:320px;
  background:#ffffff;
  padding:clamp(25px,5vw,60px);

  display:flex;
  flex-direction:column;
  justify-content:center;
}

/* RIGHT SECTION */

.right-side{
  flex:1;
  min-width:320px;

  background:#dfece7;

  display:flex;
  justify-content:center;
  align-items:center;

  padding:clamp(25px,5vw,50px);
}

/* LOGO */

.logo-box{
  width:70px;
  height:70px;

  border-radius:20px;

  background:linear-gradient(135deg,#16c79a,#246bff);

  color:#fff;

  display:flex;
  justify-content:center;
  align-items:center;

  font-size:28px;

  margin-bottom:30px;

  box-shadow:0 10px 25px rgba(0,0,0,0.08);
}

/* TITLES */

.main-title{
  font-size:clamp(32px,5vw,58px);
  font-weight:800;
  color:#222;
  line-height:1.2;
  text-transform:uppercase;
  margin-bottom:15px;
}

.sub-title{
  font-size:clamp(18px,2vw,22px);
  color:#7b7b7b;
  margin-bottom:50px;
}

/* FEATURES */

.feature-item{
  display:flex;
  gap:18px;
  margin-bottom:30px;

  padding:18px;
  border-radius:18px;

  transition:0.3s ease;
}

.feature-item:hover{
  background:#f8f8f8;
  transform:translateY(-3px);
}

.feature-icon{
  width:55px;
  height:55px;

  border-radius:15px;

  background:#e9f5ef;
  color:#11a76d;

  display:flex;
  justify-content:center;
  align-items:center;

  font-size:20px;

  flex-shrink:0;
}

.feature-title{
  font-size:22px;
  font-weight:700;
  color:#222;
  margin-bottom:6px;
}

.feature-text{
  font-size:16px;
  color:#666;
  line-height:1.7;
}

/* DOTS */

.carousel-indicators{
  bottom:25px;
}

.carousel-indicators [data-bs-target]{
  width:12px;
  height:12px;

  border-radius:50%;

  background:#cfcfcf;

  border:none;

  opacity:1;

  margin:0 6px;
}

.carousel-indicators .active{
  background:#10b26f;
}

/* RIGHT CONTENT */

.right-content{
  text-align:center;
  max-width:500px;
}

.right-content i{
  font-size:clamp(90px,12vw,160px);
  color:#16b27b;
  margin-bottom:30px;
}

.right-content h2{
  font-size:clamp(28px,4vw,46px);
  font-weight:800;
  color:#222;
  margin-bottom:20px;
}

.right-content p{
  font-size:clamp(16px,2vw,20px);
  color:#666;
  line-height:1.8;
}

/* BUTTON */

.next-btn{
  margin-top:25px;

  padding:14px 30px;

  border:none;
  border-radius:14px;

  background:#10b26f;

  color:#fff;

  font-size:18px;
  font-weight:600;

  transition:0.3s;
}

.next-btn:hover{
  background:#0d955d;
}

/* TABLET */

@media(max-width:992px){

  .left-side,
  .right-side{
    padding:40px 30px;
  }

}

/* MOBILE */

@media(max-width:768px){

  .main-page{
    flex-direction:column;
  }

  .left-side,
  .right-side{
    width:100%;
  }

  .feature-item{
    gap:15px;
  }

  .logo-box{
    width:60px;
    height:60px;
    font-size:24px;
  }

}

  </style>
</head>

<body>

<!-- SLIDER -->

<div id="mainSlider"
     class="carousel slide"
     data-bs-touch="true"
     data-bs-interval="false">

  <div class="carousel-inner">

    <!-- PAGE 1 -->

    <div class="carousel-item active">

      <div class="main-page">

        <div class="left-side">

          <div class="logo-box">
            <i class="fa-solid fa-bolt"></i>
          </div>

          <h1 class="main-title">
            SMART LOCAL <br>
            SUBSCRIPTIONS
          </h1>

          <p class="sub-title">
            More local. More value.
          </p>

          <div class="feature-item">

            <div class="feature-icon">
              <i class="fa-solid fa-tag"></i>
            </div>

            <div>

              <div class="feature-title">
                Save More
              </div>

              <div class="feature-text">
                Get exclusive discounts and offers from your favorite local businesses.
              </div>

            </div>

          </div>

          <div class="feature-item">

            <div class="feature-icon">
              <i class="fa-solid fa-mug-hot"></i>
            </div>

            <div>

              <div class="feature-title">
                One Smart Plan
              </div>

              <div class="feature-text">
                Pay one monthly fee and enjoy multiple benefits every day.
              </div>

            </div>

          </div>

          <div class="feature-item">

            <div class="feature-icon">
              <i class="fa-solid fa-store"></i>
            </div>

            <div>

              <div class="feature-title">
                Support Local
              </div>

              <div class="feature-text">
                Support local businesses and enjoy a better community.
              </div>

            </div>

          </div>

          <button class="next-btn"
                  data-bs-target="#mainSlider"
                  data-bs-slide="next">
            Next
          </button>

        </div>

        <div class="right-side">

          <div class="right-content">

            <i class="fa-solid fa-mobile-screen-button"></i>

            <h2>
              Responsive Design
            </h2>

            <p>
              Optimized for Desktop, Tablet, and Mobile devices with a fully flexible layout.
            </p>

          </div>

        </div>

      </div>

    </div>

    <!-- PAGE 2 -->

    <div class="carousel-item">

      <div class="main-page">

        <div class="left-side">

          <div class="logo-box">
            <i class="fa-solid fa-city"></i>
          </div>

          <h1 class="main-title">
            SMART <br>
            CITY PLANS
          </h1>

          <p class="sub-title">
            One subscription for your entire city.
          </p>

          <div class="feature-item">

            <div class="feature-icon">
              <i class="fa-solid fa-ticket"></i>
            </div>

            <div>

              <div class="feature-title">
                Daily Offers
              </div>

              <div class="feature-text">
                Unlock premium local deals every single day.
              </div>

            </div>

          </div>

          <div class="feature-item">

            <div class="feature-icon">
              <i class="fa-solid fa-wallet"></i>
            </div>

            <div>

              <div class="feature-title">
                Save Money
              </div>

              <div class="feature-text">
                Spend less while enjoying more experiences.
              </div>

            </div>

          </div>

          <button class="next-btn"
                  data-bs-target="#mainSlider"
                  data-bs-slide="next">
            Continue
          </button>

        </div>

        <div class="right-side">

          <div class="right-content">

            <i class="fa-solid fa-building"></i>

            <h2>
              Your Smart City
            </h2>

            <p>
              Discover restaurants, cafés, gyms and more through one smart membership.
            </p>

          </div>

        </div>

      </div>

    </div>

    <!-- PAGE 3 -->

    <div class="carousel-item">

      <div class="main-page">

        <div class="left-side">

          <div class="logo-box">
            <i class="fa-solid fa-store"></i>
          </div>

          <h1 class="main-title">
            SUPPORT <br>
            LOCAL BUSINESS
          </h1>

          <p class="sub-title">
            Better communities start locally.
          </p>

          <div class="feature-item">

            <div class="feature-icon">
              <i class="fa-solid fa-heart"></i>
            </div>

            <div>

              <div class="feature-title">
                Community First
              </div>

              <div class="feature-text">
                Every purchase helps local businesses grow stronger.
              </div>

            </div>

          </div>

          <button class="next-btn">
            Get Started
          </button>

        </div>

        <div class="right-side">

          <div class="right-content">

            <i class="fa-solid fa-handshake"></i>

            <h2>
              Grow Together
            </h2>

            <p>
              Build stronger connections with your neighborhood businesses.
            </p>

          </div>

        </div>

      </div>

    </div>

  </div>

  <!-- DOTS -->

  <div class="carousel-indicators">

    <button type="button"
            data-bs-target="#mainSlider"
            data-bs-slide-to="0"
            class="active">
    </button>

    <button type="button"
            data-bs-target="#mainSlider"
            data-bs-slide-to="1">
    </button>

    <button type="button"
            data-bs-target="#mainSlider"
            data-bs-slide-to="2">
    </button>

  </div>

</div>

<!-- Bootstrap JS -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.8/dist/js/bootstrap.bundle.min.js"></script>

</body>
</html>
