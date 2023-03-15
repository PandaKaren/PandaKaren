<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Pandas</title>
  </head>
  <style>
    body {
      background: linear-gradient(to bottom, #e6d3a7, #3a7563, #392f2f);
      background-repeat: no-repeat;
      background-attachment: fixed;
    }
    h1 {
      color: #59a985;
      font-size: 72px;
      font-weight: bold;
      text-align: center;
      padding-bottom: 0px;
      margin: 10px;
    }
    .green {
      clear: both;
      color: green;
      background-color: green;
      height: 3px;
      border-width: 0;
      margin: 0px 10px 0px 10px;
    }
    h2 {
      font-weight: 20px;
      text-align: center;
    }
      .outlined {
        text-shadow: 3px 3px black, -3px -3px black, 3px -3px black, -3px 3px black;
    }
    p {
      color: black;
      border: 5px solid green;
      background: beige;
      padding: 40px 40px;
    }
    
    h4 {
      margin-bottom: 0px;
    }
    button {
      text-align: center;
      margin-top: 40px;
      margin-left: 280px;
      padding: 15px;
      color: black;
      display: block;
      background-color: #e6d3a7;
      border-width: 3px;
      border-color: black;
      border-radius: 10px;
      transition: all 200ms ease-in-out;
      box-shadow: 5px 5px 4px #392f2f;
    }
    button:hover {
      background: #392f2f;
      cursor: pointer;
      color: #ffffff;
      box-shadow: 5px 5px 4px #e6d3a7;
    }
  </style>
  <h1>
    <div class="outlined">Pandas
    </h1>
    <hr class="green">
    <h2>
      <strong>The Oreo of the Animal Kingdom</strong>
    </h2>
      <img
        src="https://cdn.creatureandcoagency.com/uploads/2014/04/Panda-Facts-Featured.jpg"
        alt="panda"
        style="
          float: left;
          margin-right: 40px;
          margin-left: 50px;
          width: 30%;
          padding-top: 26px;
        "
      />
      <p
        style="
          text-align: justify;
          margin-right: 10px;
          margin-left: 10px;
          font-size: 25px;
          padding-bottom: 40px;
        "
      >
        The panda, with its distinctive black and white coat, is adored by the
        world and considered a national treasure in China. Pandas live mainly in
        temperate forests high in the mountains of southwest China, where they
        subsist almost entirely on bamboo. They must eat around 26 to 84 pounds
        of it every day, depending on what part of the bamboo they are eating.
        They use their enlarged wrist bones that function as opposable thumbs. A
        newborn panda is about the size of a stick of butter—about 1/900th the
        size of its mother—but females can grow up to about 200 pounds, while
        males can grow up to about 300 pounds as adults. These bears are
        excellent tree climbers despite their bulk.
        <br>
  <div style="display: flex">
    <div
      style="
        border: 5px solid green;
        background-color: beige;
        padding: 20px;
        flex: 1;
        margin-right: 10px;
        margin-left: 10px;
        text-align: center;
        font-size: 20px;
      "
    >
      <h3>For more information, click here:</h3>

      <p2>
        <a href="https://www.worldwildlife.org/species/giant-panda"
          ><img
            src="data:image/png;base64,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"
            alt="Pandas"
            width="150px"
        /></a>
      </p2>
    </div>
    <div
      style="
        border: 5px solid green;
        background-color: beige;
        padding: 20px;
        flex: 1;
        margin-right: 10px;
        margin-left: 10px;
        text-align: center;
        font-size: 20px;
      "
    >
      <h4>Sign Up for More Animals in Your Inbox!</h40>
      <br />
      <p3>
        <button id="myButton">Click Here!</button>
      </p3>
    </div>
  </div>

  <script>
    function apply() {
      let name = prompt("What is your name?");
      let age = prompt("How old are you?");
      let email = prompt("What is your email");

      if (age >= 15) {
        alert(
          "Hi " +
            name +
            "!" +
            " We will email you more weekly animals at: " +
            email +
            ". Thank you for joining us. Visit the teaching resources page on the WWF website for things to do in the classroom."
        );
      } else {
        alert(
          "Hi " +
            name +
            "!" +
            " We will email you more weekly animals at: " +
            email +
            ". Thank you for joining us."
        );
      }
    }
    let applyButton = document.querySelector("button");
    applyButton.addEventListener("click", apply);
  </script>
</html>
