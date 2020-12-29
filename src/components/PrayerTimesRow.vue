<template>
  <div class="prayerTime">
      
      <div class="prayerTimeRow">
          <div class="title">{{ timeLabel }}</div>
          <div class="time">{{ timeLeft }}</div>
      </div>
      <div class="congregationTimeRow">
          <div class="time">{{ timeRight }}</div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'PrayerTimesRow',
    props: {
        timeLeft: {
            type: String,
            required: false
        },
        timeRight: {
            type: String,
            required: false
        },
        timeLabel: {
            type: String,
            required: false
        },

    }
}
</script>

<style scoped>
    .prayerTime{
        display: grid;
        grid-template-columns: 50% 50%;
        border: 1px solid navy;
        font-size: .5rem
    }

    .prayerTimeRow {
        display: grid;
        grid-template-columns: 25% 75%;
    }
</style>