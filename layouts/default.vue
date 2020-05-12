<template>
  <div>
    <header>
      <div class="logo"><h1>LOGO</h1></div>
      <div class="headerlinks">
        <a href="" class="headerlink__getticket headerlinks--nobg">
          I didn't get my tickets
        </a>
        <a href="" class="headerlink__createevent headerlinks--bg">
          create your own event
        </a>
      </div>
    </header>
    <nuxt />
  </div>
</template>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background-color: #f2f2f2;
}
a{
  display: inline-block;
  text-decoration: none;
}
img{
  width: 100%;
  height: 100%;
}
*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
header{
    max-width: 90%;
    margin: 2.5% auto;
    display:flex;
    flex-direction: row;
    justify-content: space-between;
}
.headerlinks{
    text-transform: capitalize;
    width: 50%;
    overflow: auto;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    font-weight: bold;
}
.headerlinks--nobg{
  display: block;
    color: #000;
    padding: 0 5%;
}
.headerlinks--bg{
  display: block;
  width: max-content;
  overflow: auto;
  border-radius: 4.06693px;
  background-color: #f5a623;
  color:#fff;
  padding: 2.5% 5%;
}

.button--orange {
  display: inline-block;
  border-radius: 4px;
  color: #fff;
  text-decoration: none;
  padding: 10px 30px;
  background: #f5a623;
}

.button--orange:hover {
  color: #fff;
  background-color: #fff;
  color: #f5a623;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

</style>
