<script>
  import svelteLogo from "./assets/svelte.svg";
  import viteLogo from "/vite.svg";
  import Counter from "./lib/Counter.svelte";
  import logo from "./logo.png";
  import GitHubCorner from "./GitHubCorner.svelte";
  
</script>
<main>
  
  <body>
    <GitHubCorner
      href="https://github.com/yashbhangale"
      fill="#7a3277"
      color="#fff"
    />

    <link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css" />
    <link
      rel="stylesheet"
      href="https://www.w3schools.com/lib/w3-theme-light-blue.css"
    />

    <!-- Content container -->

    <div class="container">
      <!-- Image and name container. Change to your picture here. -->
      <div class="" style="text-align: center">
        <p class="name">
          <span
            class="w3-padding w3-theme-l1 w3-margin w3-round"
            style="font-weight: bolder; font-size: x-large; border: 3px solid #000000a2;"
            >Yash Bhangale!</span
          >
        </p>
        <img
          src={logo}
          class="w3-round"
          alt="person image"
          width="150px"
          height="150px"
          style="border-radius: 50%; border: 5px solid darkblue !important; margin-top: 16px;"
        />

        <p>
          <span
            class="profession w3-padding w3-theme-d5 w3-round"
            style="font-weight: bolder; border: 2px solid #1a3946;"
            >I am an Engineering Student!</span
          >
        </p>
      </div>
      
      <!-- Links section 1. Replace the # inside of the "" with your links. -->
      <div class="links-container">
      <div class="icons w3-padding">
          <a href="https://github.com" target="_blank">
            <i data-feather="github" />
          </a>
          <a href="#" target="_blank">
            <i data-feather="linkedin" />
          </a>
          <a href="#" target="_blank">
            <i data-feather="youtube" />
          </a>
          <a href="#" target="_blank">
            <i data-feather="twitter" />
          </a>
          <a href="#" target="_blank">
            <i data-feather="link-2" />
          </a>
          <style>
            .icons a svg {
              fill: darkblue;
              transform: scale(1.5);
            }
            .icons {
              display: flex;
              gap: 40px;
            }
          </style>
        </div>
        <a
          href="#"
          class="w3-button w3-round w3-theme-d3 w3-border link"
          target="_blank">Projects</a
        >
        <br />
        <a
          href="#"
          class="w3-button w3-round w3-theme-d3 w3-border link"
          target="_blank">MY BLOG</a
        >
        <br />
        <a
          href="#"
          class="w3-button w3-round w3-theme-d3 w3-border link"
          target="_blank">Github</a
        >
        <br />
        <p>
          <span
            class="subscribe w3-padding w3-theme-d5 w3-round"
            style="font-weight: bolder; border: 3px solid darkblue ;"
            >Subscribe to my news!</span
          >
        </p>
        <div class="submit" style="width: 80%;">
          <form>
            <input
              class="w3-input w3-round w3-theme-d3 w3-border"
              type="text"
              placeholder="Your email . . . "
              name="email"
            />
            <script>
              function openMailApp() {
                window.location.href = "mailto:youremail@example.com";
              }
            </script>

            <button
              class="w3-button w3-round w3-border"
              type="submit"
              on:click={openMailApp}>SUBSCRIBE</button
            >
          </form>
        </div>
        <br />
      </div>
    </div>
    <script>
      feather.replace();
    </script>
  </body>
</main>

<style>
  .container {
    width: 100%;
    height: 100%;
    padding-right: 15px;
    padding-left: 15px;
    margin-right: auto;
    margin-left: auto;
  }

  .name {
    margin-top: 50px !important;
  }

  .w3-theme-d3 {
    background-color: rgba(27, 100, 129, 0.856) !important;
    border-radius: 8px !important;
  }

  .w3-theme-d3:hover {
    background-color: rgb(12, 186, 255) !important;
  }

  a {
    font-size: x-large;
  }

  .w3-border {
    border: 3px solid #ccc !important;
  }

  .links-container {
    display: flex;
    flex-direction: column;
    jusify-content: center;
    align-items: center;
  }

  .links-container a {
    width: 80%;
  }

  .profession {
    font-size: 15px;
  }

  .subscribe {
    font-size: 15px;
  }

  .submit form {
    display: flex;
    flex-direction: column;
  }

  .submit form button {
    margin-top: 5px;
    background-color: rgba(27, 122, 159, 0.9) !important;
    color: #fff !important;
  }

  .submit form button:hover {
    background-color: rgba(15, 67, 87, 0.9) !important;
    color: #fff !important;
  }
  .submit form input {
    width: 100% !important;
  }
  .submit form input::placeholder {
    color: #fff;
  }

  .icons a {
    text-decoration: none;
  }

  @media screen and (min-width: 768px) {
    .link {
      width: 100%;
    }
  }
  @media screen and (min-width: 576px) {
    .container {
      max-width: 540px;
    }

    .profession {
      font-size: 24px;
    }
  }
</style>
