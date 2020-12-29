<template>
  <div class="prayerTime">
      
      <div class="prayerTimeRow">
          <div class="title"></div>
          <div class="time">Athan</div>
      </div>
      <div class="congregationTimeRow">
          <div class="time">Iqamah</div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'PrayerTimesRowHeader',
}
</script>

<style scoped>
    .prayerTime{
        display: grid;
        grid-template-columns: 50% 50%;
        border: 1px solid navy;
        background-color:navy;
        color: white;
        font-size: 0.5rem
    }

    .prayerTimeRow {
        display: grid;
        grid-template-columns: 25% 75%;
    }
</style>