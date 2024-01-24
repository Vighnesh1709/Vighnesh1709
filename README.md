<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <link rel="stylesheet" href="open.css" />
    <script>
      function openUp() {
        const $opentop = document.querySelector("#opentop");
        const $top = document.querySelector("#top");
        const $front = document.querySelector("#front");
        const $back = document.querySelector("#back");
        const $letter = document.querySelector("#letter");
        const $button = document.querySelector("button");

        $opentop.beginElement();
        $top.style.zIndex = 2;

        $top.classList.add("animate");
        $front.classList.add("animate");
        $back.classList.add("animate");
        $button.classList.add("animate");
        $letter.classList.add("animate");
      }
    </script>
  </head>
  <body>
    <div class="text">
      <h1>Hey ! Listen this is for you 💖....</h1>
    </div>
    <div id="envelope">
      <div id="back">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          height="300"
          width="300"
        >
          <polygon
            points="0,100 300,100 300,300 0,300"
            style="fill: #4a274a; stroke: none; stroke-width: 0"
          />
        </svg>
      </div>
      <div id="front">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          height="300"
          width="300"
        >
          <polygon
            points="0,100 150,200 300,100 300,300 0,300"
            style="fill: #2abad0; stroke: #ffffff; stroke-width: 3"
          />
        </svg>
      </div>
      <div id="top">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          height="300"
          width="300"
        >
          <polygon
            points="0,100 150,200 300,100"
            style="fill: #2abad0; stroke: #ffffff; stroke-width: 2"
          >
            <animate
              id="opentop"
              attributeName="points"
              dur="0.5s"
              fill="freeze"
              begin="indefinite"
              from="0,100 150,200 300,100"
              to="0,100 150,0 300,100"
            />
          </polygon>
        </svg>
      </div>

      <div id="letter">
        <h1>For My <span>Love</span></h1>

        <!-- <img src="https://i.postimg.cc/5yZQnDpb/ukraine-7424066-640.webp" />-->
        <p>
          Is Jalebi the swetest? 
         Or is it Gulab Jamun?
          Nah You are the sweetest
         Shall we get you something spicy (like Panipuri) to balance it out?
          <br />
          If You Accept
          <a href="new.html">Click Here</a>
        </p>
      </div>
      <button onclick="openUp()">Click Here</button>
    </div>
  </body>
</html>
