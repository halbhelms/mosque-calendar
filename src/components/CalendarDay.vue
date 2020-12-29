<template>
    <div class="day">
        <div class="date">{{ date }}</div>
        
        <div v-if="!isEmpty" class="_prayerTimes">
            <PrayerTimesRowHeader />
            <PrayerTimesRow timeLeft="4.23" timeRight="5.15" timeLabel="F"/>
            <PrayerTimesRow timeLeft="4.23" timeRight="5.15" timeLabel="S"/>
            <PrayerTimesRow timeLeft="4.23" timeRight="5.15" timeLabel="D"/>
            <PrayerTimesRow timeLeft="4.23" timeRight="5.15" timeLabel="A"/>
            <PrayerTimesRow timeLeft="4.23" timeRight="5.15" timeLabel="M"/>
            <PrayerTimesRow timeLeft="4.23" timeRight="5.15" timeLabel="I"/>
        </div>
  </div>
</template>

<script>
import PrayerTimesRow from './PrayerTimesRow'
import PrayerTimesRowHeader from './PrayerTimesRowHeader'
export default {
    name: 'CalendarDay',
    components: { PrayerTimesRow, PrayerTimesRowHeader },
    props: {
        isEmpty: {
            type: Boolean,
            required: false
        },
        date: {
            type: String,
            required: true
        }
    }
}
</script>

<style>
    .day {
       display: grid;
       grid-template-columns: 30% 70%;
       outline: 1px solid navy;
    }

    ._prayerTimes {
    }
</style>