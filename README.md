<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Karamlyy</title>
    <link rel="stylesheet" href="style.css" />
    <script
      src="https://kit.fontawesome.com/f6816dd194.js"
      crossorigin="anonymous"
    ></script>
  </head>
  <body>
    <div class="main center">
      <div class="main_container center">
        <div class="sub_container active">
          <div id="home">
            <!-- header -->
            <header class="center">
              <div class="logo">
                <p>karamlyy</p>
              </div>
              <div class="chat">
                <i class="fab fa-rocketchat"></i>
              </div>
            </header>
            <!-- posts -->
            <div class="post_container containers active">
              <div class="post">
                <img src="photo5299011950249883055.jpg" alt="" srcset="" />
                <div class="post_footer center">
                  <div class="center">
                    <img src="u5rraa.jpg" alt="" srcset="" />
                    <p>@karamlyy</p>
                  </div>
                  <div class="center">
                    <i class="far fa-heart"></i>
                    <i class="far fa-comment-dots"></i>
                    <i class="fas fa-arrow-right"></i>
                  </div>
                </div>
              </div>
              <div class="post">
                <img src="photo5299011950249883056.jpg" alt="" srcset="" />
                <div class="post_footer center">
                  <div class="center">
                    <img src="u5rraa.jpg" alt="" srcset="" />
                    <p>@karamlyy</p>
                  </div>
                  <div class="center">
                    <i class="far fa-heart"></i>
                    <i class="far fa-comment-dots"></i>
                    <i class="fas fa-arrow-right"></i>
                  </div>
                </div>
              </div>
              <div class="post">
                <img src="photo5299011950249883057.jpg" alt="" srcset="" />
                <div class="post_footer center">
                  <div class="center">
                    <img src="u5rraa.jpg" alt="" srcset="" />
                    <p>@karamlyy</p>
                  </div>
                  <div class="center">
                    <i class="far fa-heart"></i>
                    <i class="far fa-comment-dots"></i>
                    <i class="fas fa-arrow-right"></i>
                  </div>
                </div>
              </div>
              <div class="post">
                <img src="photo5299011950249883058.jpg" alt="" srcset="" />
                <div class="post_footer center">
                  <div class="center">
                    <img src="u5rraa.jpg" alt="" srcset="" />
                    <p>@karamlyy</p>
                  </div>
                  <div class="center">
                    <i class="far fa-heart"></i>
                    <i class="far fa-comment-dots"></i>
                    <i class="fas fa-arrow-right"></i>
                  </div>
                </div>
              </div>
              <div class="post">
                <img src="photo5299011950249883059.jpg" alt="" srcset="" />
                <div class="post_footer center">
                  <div class="center">
                    <img src="u5rraa.jpg" alt="" srcset="" />
                    <p>@karamlyy</p>
                  </div>
                  <div class="center">
                    <i class="far fa-heart"></i>
                    <i class="far fa-comment-dots"></i>
                    <i class="fas fa-arrow-right"></i>
                  </div>
                </div>
              </div>
              <div class="post">
                <img src="IMG_20210831_221724_774.jpg" alt="" srcset="" />
                <div class="post_footer center">
                  <div class="center">
                    <img src="u5rraa.jpg" alt="" srcset="" />
                    <p>@karamlyy</p>
                  </div>
                  <div class="center">
                    <i class="far fa-heart"></i>
                    <i class="far fa-comment-dots"></i>
                    <i class="fas fa-arrow-right"></i>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="browse"></div>
        <div class="likes"></div>
        <div class="profile"></div>
        <div class="nav center">
          <div class="box center">
            <input
              type="checkbox"
              name=""
              class="tab"
              id=""
              checked
              value="home"
            />
            <i class="fas fa-home"></i>
            <p>Home</p>
          </div>
          <div class="box center">
            <input type="checkbox" name="" class="tab" id="" value="browse" />
            <i class="fas fa-globe-europe"></i>
            <a href="explore.html"><p>Explore</p></a>
          </div>
          <div class="box center">
            <input type="checkbox" name="" class="tab" id="" value="likes" />
            <i class="fas fa-heart"></i>
            <p>Notification</p>
          </div>
          <div class="box center">
            <input type="checkbox" name="" class="tab" id="" value="profile" />
            <i class="fas fa-user-circle"></i>
            <p>Profile</p>
          </div>
        </div>
      </div>
    </div>
    <script>
      const tab = document.querySelectorAll(".tab");
      const sub = document.querySelector(".sub_container");
      const likes = document.querySelector(".likes");
      const browse = document.querySelector(".browse");
      const profile = document.querySelector(".profile");
      //   const containers = document.querySelector(".sub_container");
      //   const containers = document.querySelector(".sub_container");
      tab.forEach((e) => {
        e.addEventListener("click", (event) => {
          tab.forEach((e) => {
            e.checked = false;
          });
          event.target.checked = true;
          sub.classList.remove("active");
          browse.classList.remove("active");
          likes.classList.remove("active");
          profile.classList.remove("active");
          if (event.target.value == "home") {
            sub.classList.add("active");
          } else if (event.target.value == "browse") {
            browse.classList.add("active");
          } else if (event.target.value == "likes") {
            likes.classList.add("active");
          } else if (event.target.value == "profile") {
            profile.classList.add("active");
          }
        });
      });
    </script>
  </body>
</html>
