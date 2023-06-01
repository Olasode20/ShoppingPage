<template>
<div className="box">
  <div className="head">
    <h1 className="top">ASUS</h1>
    <nav>
      <ul>
        <li><a href="#" className="active">Home</a></li>
        <li><a href="#">Gallery</a></li>
        <li><a href="#">Colllections</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </div>
  <div className="body">
    <div className="left-body">
      <h1> Quality apparel without the price tag</h1>
      <p className="subhead"> You don't need to check the price before you get to purchase our items. You can
        always check out our collections with a wide variety of nice wears. </p>
    <div className="section">
      <a href="#" className="prm-btn">Browse our collection</a>
       <a href="#" className="sec-btn">
         <span>Spring '23 collections >>> </span></a>
    </div>
    <div className="customer">
      <p className="employee"> 50K </p>
      <p className="details"> We are proud of our customers and we are still willing to gain more trust as our products are
        top-notch. We sell quality wears and very trust-worthy.</p>
    </div>
    </div>
    <div className="right-body">
        <div className="card card1">
          <div className="card-details">
    <div className="shoe-details">
          <a href="#"> Fauxica Sport </a>
          <p> Running Shoe</p>
          </div>
          <p className="shoe-price">$45</p>
          </div>
        </div>
        <div className=" card card2">
          <div className="card-details">
    <div className="shoe-details">
          <a href="#"> Fauxica Sport </a>
          <p> Running Shoe</p>
          </div>
          <p className="shoe-price">$45</p>
          </div>
        </div>
        <div className="card card3">
          <div className="card-details">
    <div className="shoe-details">
          <a href="#"> Fauxica Sport </a>
          <p> Running Shoe</p>
          </div>
          <p className="shoe-price">$45</p>
        </div>
        </div>
      </div>
  </div>
</div>

</template>



<script>
export default {};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Geologica:wght@300&family=Source+Serif+Pro&display=swap");

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

html {
  font-size: 90%;
}

.box {
  max-width: 1000px;
  margin: 0 auto;
}

.head {
  display: flex;
  justify-content: space-between;
  line-height: 100%;
  align-items: center;
}

nav ul {
  list-style-type: none;
  display: flex;
  justify-content: space-between;
  gap: 3rem;
}

nav ul li a {
  text-decoration: none;
  text-transform: uppercase;
  color: black;
  font-size: 1rem;
  position: relative;
  font-weight: bold;
  font-family: "Geologica", sans-serif;
}

nav ul li a.active:before {
  position: absolute;
  content: "";
  width: 35%;
  height: 1px;
  border-bottom: 2px solid black;
  bottom: -6px;
}

nav ul li a:before {
  position: absolute;
  content: "";
  width: 0;
  height: 1px;
  border-bottom: 2px solid black;
  bottom: -6px;
  transition: width 0.3s;
}

nav ul li a:hover:before {
  width: 35%;
}

.body {
  display: flex;
  justify-content: space-between;
  gap: 4em;
  margin-top: 6.5em;
}

.left-body {
  width: 45%;
}

.right-body {
  flex-grow: 1;
}

.top {
  font-size: 2.8em;
}

h1 {
  font-size: 2.8em;
  margin: 0;
  font-family: "Geologica", sans-serif;
}

.subhead {
  font-size: 1em;
  font-family: "Source Serif Pro", serif;
}

.section {
  display: flex;
  gap: 1.5em;
  margin-top: 3em;
}

.prm-btn {
  background-color: rgb(245, 200, 116);
  border-radius: 1.2em;
  font-size: 1em;
  padding: 1em 2em;
  color: black;
  text-decoration: none;
  font-weight: bold;
  font-family: "Geologica", sans-serif;
}

.sec-btn {
  margin: 0 auto;
  padding: 1em 1em;
  text-decoration: none;
  font-weight: bold;
  color: black;
  font-family: "Geologica", sans-serif;
}
.customer {
  display: flex;
  margin-top: 3em;
  border: 0.1em solid black;
  border-radius: 1em;
  padding: 1.5em 1.5em;
  gap: 0.5em;
  line-height: 100%;
}

.employee {
  font-size: 1.7em;
  font-weight: bold;
}

.details {
  align-items: center;
  font-family: "Source Serif Pro", serif;
}

.right-body {
  display: grid;
  gap: 2em;
  grid-template-columns: repeat(2, auto);
  grid-template-areas:
    "left right"
    "left bottom";
}

.card {
  border: 0.1em solid black;
  border-radius: 0.5em;
  padding: 0.8em;
  display: flex;
  align-items: end;
  background-size: 145%;
  transition: background-size 0.5s;
}

.card1 {
  grid-area: left;
  background-color: rgb(182, 182, 248);
  background-image: url("./images/first.jpg");
}

.card2 {
  background-image: url("./images/second.jpg");
}

.card3 {
  background-image: url("./images/third.jpg");
}

.card-details {
  background-color: white;
  border-radius: 0.8em;
  width: 100%;
  display: flex;
  justify-content: space-between;
  padding: 0.8em 0.8em;
  align-items: center;
  transition: transform 800ms;
}

.card-details a {
  text-decoration: none;
  font-weight: bold;
  font-size: 1em;
  color: black;
  font-family: "Geologica", sans-serif;
}

.shoe-details p {
  font-size: 0.85em;
  margin: 0;
  font-family: "Source Serif Pro", serif;
}

.shoe-price {
  font-size: 1em;
  font-weight: bold;
  font-family: "Geologica", sans-serif;
}

.prm-btn:hover {
  background-color: orange;
}

.sec-btn:hover {
  text-decoration: underline;
}

.card:hover {
  background-size: 160%;
}

.card:hover .card-details {
  transform: translateY(-1em);
}
</style>
