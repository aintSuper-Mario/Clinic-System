<script>
import FullCalendar from '@fullcalendar/vue3'
import dayGridPlugin from '@fullcalendar/daygrid'
import TimeGridPlugin from '@fullcalendar/timegrid'
import InteractionPlugin from '@fullcalendar/interaction'
import ListPlugin from '@fullcalendar/list'

export default {
  components: {
    FullCalendar 
  },
  data: function() {
    return {
      calendarOptions: {
        plugins: [
            dayGridPlugin,
            TimeGridPlugin,
            InteractionPlugin,
            ListPlugin

        ],
        initialView: 'dayGridMonth',
        weekends: false,
        events: [
          { title: 'Appointment', start: new Date() }
        ]
      }
    }
  }
}
</script>

<template>
  <h2>Appointment Booking</h2>
  <FullCalendar :options='calendarOptions' />
</template>

<style scoped>
 h2 {
    color: #0146ae;
    font-weight: 800;

 }


</style>