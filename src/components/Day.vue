<template>
  <div>
    <slot name="back">
      <back-to-calendar :year="year"></back-to-calendar>
    </slot>
    <h1 class="headline">{{ date.format('DD. MMMM YYYY') }}</h1>
    <main class="page-content">
      <slot name="page-content" class="page-content"></slot>
    </main>
  </div>
</template>

<script>
import moment from 'moment';
import 'moment/locale/es';

moment.locale('es');
export default {
  name: 'Day',
  props: ['day'],
  computed: {
    date() {
      return moment(this.day, 'DD.MM.YYYY');
    },
    year() {
      return this.date.format('YYYY');
    }
  }
}
</script>

<style lang="scss">
.page-content {
  width: 50%;
  margin: 0 auto;
  flex-flow: column;
  text-align: center;
  background: rgba(#000, 0.3);
  padding: 25px;
  @media screen and (max-width: 900px) {
    width: 75%;
  }
  @media screen and (max-width: 400px) {
    width: 90%;
  }
}
</style>

