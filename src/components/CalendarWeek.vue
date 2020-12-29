<template>
  <div class="week">
      <CalendarDay :isEmpty="true" date="30"/>
      <CalendarDay date="1"/>
      <CalendarDay date="2"/>
      <CalendarDay date="3"/>
      <CalendarDay date="4"/>
      <CalendarDay date="5"/>
      <CalendarDay date="6"/>
  </div>
</template>

<script>
import CalendarDay from './CalendarDay'
export default {
    components: { CalendarDay }

}
</script>

<style>
    .week {
        display: grid;
        grid-template-columns: repeat(7, 1fr);
        grid-gap:6px
    }
</style>