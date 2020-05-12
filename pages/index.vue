<template>
  <div class="container">
    <section>
      <h1 class="title">
        The best events happening now
      </h1>
      <div class="eventlist">
        <div class="eventcard">
        <div class="eventcard__image">
            <img src="~/assets/pic.jpg" alt="">
        </div>
        <div class="eventcard__desc">
            <p class="eventcard__date">

            </p>
            <p class="eventcard__title">

            </p>
            <p class="eventcard__fee">

            </p>
        </div>
    </div>
      </div>
    </section>
  </div>
</template>

<script>
import axios from '@nuxtjs/axios';
export default {
  components: {
  },
  data() {
    return {
      events: [],
      date: '',
      title : '',
      fee : ''
    }
  },
  created() {
        const response = await axios.get('https://eventsflw.herokuapp.com/v1/events')
        .then(response =>{
          this.events = response.data;
          console.log(events);
        })
        .catch (e => {
        this.errors.push(e);
        console.log(errors);
      })
    },
  }
</script>

<style>
.container {
  max-width: 1440px;
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: #F2F2F2;
}

.eventcard{
    width: 30%;
    height:400px;
}
.eventcard__image{
    width: 100%;
    height: 300px;
}
</style>
