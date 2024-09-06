<template>
  <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
  />
  <div class="banner-1">
    <!-- NavBar -->
    <nav
      class="container px-6 mx-auto md:flex md:justify-between md:items-center"
    >
      <div class="flex items-center justify-between">
        <!-- Mobile menu button -->
        <div @click="showMenu = !showMenu" class="flex md:hidden">
          <button
            type="button"
            class="text-white hover:text-gray-400 focus:outline-none focus:text-gray-400"
          >
            <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
              <path
                fill-rule="evenodd"
                d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"
              ></path>
            </svg>
          </button>
        </div>
      </div>
      <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
      <ul
        :class="showMenu ? 'flex' : 'hidden'"
        class="flex-col items-center mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0"
      >
        <li class="menu-button"><a href="#">Home</a></li>
        <li class="menu-button"><a href="#work" v-smooth-scroll>Works</a></li>
        <li class="menu-button"><a href="#about" v-smooth-scroll>About</a></li>
        <li class="menu-button">
          <a href="#contact" v-smooth-scroll>Contact</a>
        </li>
      </ul>
    </nav>
    <!-- End Navbar -->

    <div
      class="flex flex-col md:flex-row items-center md:items-center"
      style="height: 80vh"
    >
      <!-- Text Section -->
      <div
        class="w-full md:w-6/12 space-y-5 md:space-y-10 flex flex-col justify-center items-center md:items-start md:pl-10"
        style="padding-top: 50px"
      >
        <h1
          class="3xl:text-8xl 2xl:text-7xl xl:text-6xl lg:text-4xl md:text-3xl sm:text-3xl text-xl font-bold leading-tight text-center md:text-left"
          style="color: aliceblue; font-family: Arial, Helvetica, sans-serif"
        >
          It's
          <a
            href="https://www.linkedin.com/in/arcayl-maisog-809891306/"
            target="_blank"
            class="hover:underline"
            style="color: azure"
          >
            Arcayl Maisog </a
          ><br />
          Web Programmer
        </h1>
      </div>

      <!-- Image Section -->
      <div
        class="w-full md:w-6/12 flex justify-center"
        style="padding-top: 50px"
      >
        <img
          class="3xl:h-[800px] 2xl:h-[650px] xl:h-[550px] lg:h-[550px] md:h-[450px] sm:h-[350px]"
          src="./assets/profile.png"
          alt="user image"
          style="
            height: 500px;
            border-radius: 10px;

            object-fit: cover;
          "
        />
      </div>
    </div>
  </div>

  <div class="banner-2 space-y-10 pb-20">
    <h3 class="heading3 my-5 text-center" style="color: #8ff33c">Skills</h3>
    <div
      class="card"
      style="
        background-color: transparent;
        background: radial-gradient(
          circle,
          rgba(0, 0, 0, 1) 0%,
          rgba(0, 0, 0, 1) 100%
        );
      "
    >
      <!-- Cards Wrapper -->
      <div
        class="grid gap-4 md:grid-cols-4 sm:grid-cols-1"
        style="padding: 10px"
      >
        <!-- Programming Languages Card -->
        <div
          class="py-8 px-8 md:py-16 md:px-10"
          style="
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            background-color: transparent;
            background: radial-gradient(
              circle,
              rgba(0, 0, 0, 1) 0%,
              rgba(0, 0, 0, 1) 100%
            );
          "
        >
          <h4 style="color: #8ff33c">Programming Languages</h4>
          <p style="color: #eeeeee">PHP, JavaScript</p>
        </div>
        <!-- Markup and Styling Languages Card -->
        <div
          class="py-8 px-8 md:py-16 md:px-10"
          style="
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            background-color: transparent;
            background: radial-gradient(
              circle,
              rgba(0, 0, 0, 1) 0%,
              rgba(0, 0, 0, 1) 100%
            );
          "
        >
          <h4 style="color: #8ff33c">Markup and Styling Languages</h4>
          <p style="color: #eeeeee">HTML, CSS</p>
        </div>
        <!-- Query Languages Card -->
        <div
          class="py-8 px-8 md:py-16 md:px-10"
          style="
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            background-color: transparent;
            background: radial-gradient(
              circle,
              rgba(0, 0, 0, 1) 0%,
              rgba(0, 0, 0, 1) 100%
            );
          "
        >
          <h4 style="color: #8ff33c">Query Languages</h4>
          <p style="color: #eeeeee">MySQL</p>
        </div>
        <!-- Frameworks and Libraries Card -->
        <div
          class="py-8 px-8 md:py-16 md:px-10"
          style="
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            background-color: transparent;
            background: radial-gradient(
              circle,
              rgba(0, 0, 0, 1) 0%,
              rgba(0, 0, 0, 1) 100%
            );
          "
        >
          <h4 style="color: #8ff33c">Frameworks and Libraries</h4>
          <p style="color: #eeeeee">Laravel, jQuery, Bootstrap</p>
        </div>
        <!-- APIs and Other Technologies Card -->
        <div
          class="py-8 px-8 md:py-16 md:px-10 md:col-span-4"
          style="
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            background-color: transparent;
            background: radial-gradient(
              circle,
              rgba(0, 0, 0, 1) 0%,
              rgba(0, 0, 0, 1) 100%
            );
          "
        >
          <h4 style="color: #8ff33c">APIs and Other Technologies</h4>
          <p style="color: #eeeeee">
            <span style="display: block; margin-bottom: 5px"
              >Stripe (Payment Processing)</span
            >
            <span style="display: block; margin-bottom: 5px"
              >OpenStreetMap API (Location Features)</span
            >
            <span style="display: block; margin-bottom: 5px"
              >AWS (Hosting)</span
            >
            <span style="display: block; margin-bottom: 5px"
              >Cloudinary (Image Storage)</span
            >
            <span style="display: block"
              >ChatGPT and Copilot (AI Companions)</span
            >
          </p>
        </div>
      </div>
    </div>

    <h3
      class="heading3 text-center"
      style="color: #8ff33c; padding-top: 20px"
      id="work"
    >
      My Best Works
    </h3>
    <div
      class="card"
      style="
        background-color: transparent;
        display: flex;
        justify-content: center;
      "
    >
      <div
        class="card-container-wrapper"
        style="
          display: flex;
          flex-wrap: wrap;
          justify-content: center;
          gap: 40px; /* Space between cards */
          padding: 0;
          margin: 0;
        "
      >
        <div
          class="card"
          style="
            width: 100%;
            max-width: 300px;
            padding: 0;
            margin: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            background-color: transparent;
          "
        >
          <h2
            style="
              text-align: center;
              margin: 0;
              padding: 10px 0;
              background-color: transparent;
              color: #8ff33c;
            "
          >
            Quotation Automation
            <p style="color: #eeeeee">Laravel, JQuery, Ajax, Bootstrap</p>
          </h2>

          <div
            style="
              width: 100%;
              height: 400px;
              border: 3px solid #8ff33c;
              border-image: url('./assets/bg_frame.png') 30 round;
              border-radius: 6%;
            "
          >
            <img
              src="./assets/quotation.png"
              alt="Quotation"
              style="
                width: 100%;
                height: 100%;
                object-fit: cover;
                border-radius: 5%;
              "
            />
          </div>
        </div>

        <div
          class="card"
          style="
            width: 100%;
            max-width: 300px;
            padding: 0;
            margin: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            background-color: transparent;
          "
        >
          <h2
            style="
              text-align: center;
              margin: 0;
              padding: 10px 0;
              background-color: transparent;
              color: #8ff33c;
            "
          >
            E Commerce Platform
            <p style="color: #eeeeee">Laravel, JQuery, Ajax, Bootstrap</p>
          </h2>
          <div
            style="
              width: 100%;
              height: 400px;
              border: 3px solid #8ff33c;
              border-image: url('./assets/bg_frame.png') 30 round;
              border-radius: 6%;
            "
          >
            <img
              src="./assets/ecommerce.png"
              alt="E-commerce"
              style="
                width: 100%;
                height: 100%;
                object-fit: cover;
                border-radius: 5%;
              "
            />
          </div>
        </div>

        <div
          class="card"
          style="
            width: 100%;
            max-width: 300px;
            padding: 0;
            margin: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            background-color: transparent;
          "
        >
          <h2
            style="
              text-align: center;
              margin: 0;
              padding: 10px 0;
              background-color: transparent;
              color: #8ff33c;
            "
          >
            E Commerce Store Open Street Map
            <p style="color: #eeeeee">Laravel, JQuery, Ajax, Bootstrap</p>
          </h2>
          <div
            style="
              width: 100%;
              height: 400px;
              border: 3px solid #8ff33c;
              border-image: url('./assets/bg_frame.png') 30 round;
              border-radius: 6%;
            "
          >
            <img
              src="./assets/openstreet.png"
              alt="OpenStreet"
              style="
                width: 100%;
                height: 100%;
                object-fit: cover;
                border-radius: 5%;
              "
            />
          </div>
        </div>
        <div
          class="card"
          style="
            width: 100%;
            max-width: 300px;
            padding: 0;
            margin: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            background-color: transparent;
          "
        >
          <h2
            style="
              text-align: center;
              margin: 0;
              padding: 10px 0;
              background-color: transparent;
              color: #8ff33c;
            "
          >
            Funeral Home Services
            <p style="color: #eeeeee">
              Laravel, JQuery, Bootstrap, Stripe Api, AWS
            </p>
          </h2>
          <div
            style="
              width: 100%;
              height: 400px;
              border: 3px solid #8ff33c;
              border-image: url('./assets/bg_frame.png') 30 round;
              border-radius: 6%;
            "
          >
            <img
              src="./assets/funeral.png"
              alt="Funeral"
              style="
                width: 100%;
                height: 100%;
                object-fit: cover;
                border-radius: 5%;
              "
            />
          </div>
        </div>
        <div
          class="card"
          style="
            width: 100%;
            max-width: 300px;
            padding: 0;
            margin: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            background-color: transparent;
          "
        >
          <h2
            style="
              text-align: center;
              margin: 0;
              padding: 10px 0;
              background-color: transparent;
              color: #8ff33c;
            "
          >
            Pharmacy Sales Analytics
            <p style="color: #eeeeee">
              Laravel, JQuery, Ajax, Bootstrap, Chart.js
            </p>
          </h2>
          <div
            style="
              width: 100%;
              height: 400px;
              border: 3px solid #8ff33c;
              border-image: url('./assets/bg_frame.png') 30 round;
              border-radius: 6%;
            "
          >
            <img
              src="./assets/pharmacy.png"
              alt="Funeral"
              style="
                width: 100%;
                height: 100%;
                object-fit: cover;
                border-radius: 5%;
              "
            />
          </div>
        </div>
      </div>
    </div>

    <h3 class="heading3 text-center" style="color: #8ff33c; padding-top: 20px">
      Services Offered
    </h3>
    <br />
    <div
      class="card-wrapper"
      style="
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 20px; /* Space between cards */
        padding: 0;
        margin: 0;
      "
    >
      <!-- First set of cards -->
      <div
        class="card"
        style="
          width: 100%;
          max-width: 300px;
          padding-top: 0;
          margin-top: 0;
          display: flex;
          flex-direction: column;
          align-items: center;
          background-color: transparent;
        "
      >
        <div
          style="
            width: 100%;
            height: 125px;
            border: 3px solid #8ff33c;
            border-radius: 20px;
            padding: 5px;
          "
        >
          <h2
            style="
              text-align: center;
              margin: 0;
              padding: 10px 0;
              background-color: transparent;
              color: #8ff33c;
            "
          >
            Custom Website Development
            <p style="color: #eeeeee">
              Building custom websites tailored to client needs using PHP,
              JavaScript, HTML, and CSS.
            </p>
          </h2>
        </div>
      </div>

      <div
        class="card"
        style="
          width: 100%;
          max-width: 300px;
          padding-top: 0;
          margin-top: 0;
          display: flex;
          flex-direction: column;
          align-items: center;
          background-color: transparent;
        "
      >
        <div
          style="
            width: 100%;
            height: 125px;
            border: 3px solid #8ff33c;
            border-radius: 20px;
            padding: 5px;
          "
        >
          <h2
            style="
              text-align: center;
              margin: 0;
              padding: 10px 0;
              background-color: transparent;
              color: #8ff33c;
            "
          >
            Responsive Web Design
            <p style="color: #eeeeee">
              Creating mobile-friendly websites that look great on all devices.
            </p>
          </h2>
        </div>
      </div>

      <div
        class="card"
        style="
          width: 100%;
          max-width: 300px;
          padding-top: 0;
          margin-top: 0;
          display: flex;
          flex-direction: column;
          align-items: center;
          background-color: transparent;
        "
      >
        <div
          style="
            width: 100%;
            height: 125px;
            border: 3px solid #8ff33c;
            border-radius: 20px;
            padding: 5px;
          "
        >
          <h2
            style="
              text-align: center;
              margin: 0;
              padding: 10px 0;
              background-color: transparent;
              color: #8ff33c;
            "
          >
            Content Management Systems (CMS)
            <p style="color: #eeeeee">
              Building and customizing CMS platforms for easy content
              management.
            </p>
          </h2>
        </div>
      </div>

      <!-- Second set of cards -->
      <div
        class="card"
        style="
          width: 100%;
          max-width: 300px;
          padding-top: 0;
          margin-top: 0;
          display: flex;
          flex-direction: column;
          align-items: center;
          background-color: transparent;
        "
      >
        <div
          style="
            width: 100%;
            height: 125px;
            border: 3px solid #8ff33c;
            border-radius: 20px;
            padding: 5px;
          "
        >
          <h2
            style="
              text-align: center;
              margin: 0;
              padding: 10px 0;
              background-color: transparent;
              color: #8ff33c;
            "
          >
            API Development and Integration
            <p style="color: #eeeeee">
              Creating and integrating APIs to enhance website functionality.
            </p>
          </h2>
        </div>
      </div>

      <div
        class="card"
        style="
          width: 100%;
          max-width: 300px;
          padding-top: 0;
          margin-top: 0;
          display: flex;
          flex-direction: column;
          align-items: center;
          background-color: transparent;
        "
      >
        <div
          style="
            width: 100%;
            height: 125px;
            border: 3px solid #8ff33c;
            border-radius: 20px;
            padding: 5px;
          "
        >
          <h2
            style="
              text-align: center;
              margin: 0;
              padding: 10px 0;
              background-color: transparent;
              color: #8ff33c;
            "
          >
            Web Application Development
            <p style="color: #eeeeee">
              Developing dynamic web applications for various business needs.
            </p>
          </h2>
        </div>
      </div>
    </div>
  </div>

  <div
    class="banner-2 flex flex-col md:flex-row items-center md:justify-evenly"
  >
    <div
      class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-full text-center"
      id="about"
    >
      <h4 class="text-green-400 text-xl font-bold">About Me</h4>
      <p class="text-gray-200">
        I bring a proven track record of hard work and punctuality to every
        project. My passion for web development is matched only by my dedication
        to delivering quality results on time.
      </p>
      <h6 class="text-green-400 text-lg font-semibold">Education</h6>
      <p class="text-gray-200">BS Information Technology</p>
    </div>
  </div>

  <div class="banner-1 flex flex-col lg:flex-row h-full items-center">
    <div class="w-full lg:w-6/12 p-12">
      <div class="banner-1 flex h-full items-center text-gray-200">
        <div class="message">
          <h2>Contact Me<br /></h2>
          <p>
            I'm always open to discussing new projects, creative ideas, or
            opportunities to be part of your vision. Feel free to reach out!
          </p>
        </div>
      </div>
    </div>
    <div class="w-full lg:w-6/12 p-12 flex flex-col lg:flex-row items-center">
      <!-- Container for icons -->
      <div class="flex space-x-4 p-2 items-center justify-center">
        <!-- LinkedIn Icon -->
        <div class="flex items-center justify-center p-2">
          <a
            href="https://www.linkedin.com/in/arcayl-maisog-809891306"
            target="_blank"
          >
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 448 512"
              class="w-11 h-11"
            >
              <path
                fill="#8ff33c"
                d="M416 32H31.9C14.3 32 0 46.5 0 64.3v383.4C0 465.5 14.3 480 31.9 480H416c17.6 0 32-14.5 32-32.3V64.3c0-17.8-14.4-32.3-32-32.3zM135.4 416H69V202.2h66.5V416zm-33.2-243c-21.3 0-38.5-17.3-38.5-38.5S80.9 96 102.2 96c21.2 0 38.5 17.3 38.5 38.5 0 21.3-17.2 38.5-38.5 38.5zm282.1 243h-66.4V312c0-24.8-.5-56.7-34.5-56.7-34.6 0-39.9 27-39.9 54.9V416h-66.4V202.2h63.7v29.2h.9c8.9-16.8 30.6-34.5 62.9-34.5 67.2 0 79.7 44.3 79.7 101.9V416z"
              />
            </svg>
          </a>
        </div>

        <!-- GitHub Icon -->
        <div class="flex items-center justify-center p-2" id="contact">
          <a href="https://github.com/kael8" target="_blank">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 496 512"
              class="w-11 h-11"
            >
              <path
                fill="#8ff33c"
                d="M165.9 397.4c0 2-2.3 3.6-5.2 3.6-3.3 .3-5.6-1.3-5.6-3.6 0-2 2.3-3.6 5.2-3.6 3-.3 5.6 1.3 5.6 3.6zm-31.1-4.5c-.7 2 1.3 4.3 4.3 4.9 2.6 1 5.6 0 6.2-2s-1.3-4.3-4.3-5.2c-2.6-.7-5.5 .3-6.2 2.3zm44.2-1.7c-2.9 .7-4.9 2.6-4.6 4.9 .3 2 2.9 3.3 5.9 2.6 2.9-.7 4.9-2.6 4.6-4.6-.3-1.9-3-3.2-5.9-2.9zM244.8 8C106.1 8 0 113.3 0 252c0 110.9 69.8 205.8 169.5 239.2 12.8 2.3 17.3-5.6 17.3-12.1 0-6.2-.3-40.4-.3-61.4 0 0-70 15-84.7-29.8 0 0-11.4-29.1-27.8-36.6 0 0-22.9-15.7 1.6-15.4 0 0 24.9 2 38.6 25.8 21.9 38.6 58.6 27.5 72.9 20.9 2.3-16 8.8-27.1 16-33.7-55.9-6.2-112.3-14.3-112.3-110.5 0-27.5 7.6-41.3 23.6-58.9-2.6-6.5-11.1-33.3 2.6-67.9 20.9-6.5 69 27 69 27 20-5.6 41.5-8.5 62.8-8.5s42.8 2.9 62.8 8.5c0 0 48.1-33.6 69-27 13.7 34.7 5.2 61.4 2.6 67.9 16 17.7 25.8 31.5 25.8 58.9 0 96.5-58.9 104.2-114.8 110.5 9.2 7.9 17 22.9 17 46.4 0 33.7-.3 75.4-.3 83.6 0 6.5 4.6 14.4 17.3 12.1C428.2 457.8 496 362.9 496 252 496 113.3 383.5 8 244.8 8zM97.2 352.9c-1.3 1-1 3.3 .7 5.2 1.6 1.6 3.9 2.3 5.2 1 1.3-1 1-3.3-.7-5.2-1.6-1.6-3.9-2.3-5.2-1zm-10.8-8.1c-.7 1.3 .3 2.9 2.3 3.9 1.6 1 3.6 .7 4.3-.7 .7-1.3-.3-2.9-2.3-3.9-2-.6-3.6-.3-4.3 .7zm32.4 35.6c-1.6 1.3-1 4.3 1.3 6.2 2.3 2.3 5.2 2.6 6.5 1 1.3-1.3 .7-4.3-1.3-6.2-2.2-2.3-5.2-2.6-6.5-1zm-11.4-14.7c-1.6 1-1.6 3.6 0 5.9 1.6 2.3 4.3 3.3 5.6 2.3 1.6-1.3 1.6-3.9 0-6.2-1.4-2.3-4-3.3-5.6-2z"
              />
            </svg>
          </a>
        </div>
      </div>

      <div class="pt-7 lg:pt-0">
        <button
          class="btn bg-transparent text-green-400 border-2 border-green-400 rounded-full px-6 py-3 text-lg cursor-pointer transition-colors duration-300 ease-in-out"
          onclick="window.location.href='https://calendly.com/arcaylmaisog8/30min'"
        >
          Book a free consultation
        </button>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      showMenu: false,
    };
  },
};
</script>
