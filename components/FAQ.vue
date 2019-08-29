<template>
  <div id="faq-container">
    <div>
      <h1 id="faq-title"><strong>Frequently Asked Questions</strong></h1>
    </div>
    <VueFaqAccordion :items="myItems" />
  </div>
</template>

<script>
import VueFaqAccordion from 'vue-faq-accordion'

export default {
  components: {
    VueFaqAccordion
  },
  data() {
    return {
      myItems: [
        {
          title: 'How many time zones are there in all?',
          value:
            'Given a 24-hour day and 360 degrees of longitude around the Earth',
          category: 'Token'
        },
        {
          title: 'How long is a day and year on Venus?',
          value:
            'Venus takes 224.7 Earth days to complete one orbit around the Sun.',
          category: 'Token'
        },
        {
          title: 'What animal smells like popcorn?',
          value: 'Binturongs smell like popcorn.',
          category: 'Airdrop'
        }
      ],
      props: {
        /**
         * Array of items
         * Object style {questionProperty: string, answerProperty: string, tabName: string}
         * You can change object keys names using other props (questionProperty, answerProperty, tabName)
         */
        items: {
          type: Array,
          required: true
        },

        /**
         * Key name of object in items array for specifying title of question
         */
        questionProperty: {
          type: String,
          default: 'title'
        },

        /**
         * Key name of object in items array for specifying content text of open question
         */
        answerProperty: {
          type: String,
          default: 'value'
        },

        /**
         * Key name of object in items array for specifying navigation tab name
         */
        tabName: {
          type: String,
          default: 'category'
        },

        /**
         * Color for hover and active tab/question
         * possible format: 'red', '#F00', 'rgba(255, 0, 0, 1)'
         */
        activeColor: {
          type: String,
          default: '#D50000'
        },

        /**
         * Color for borders
         */
        borderColor: {
          type: String,
          default: '#9E9E9E'
        },

        /**
         * Color for fonts
         */
        fontColor: {
          type: String,
          default: '#000000'
        }
      }
    }
  }
}
</script>
<style scoped>
#faq-container {
  padding-top: 30px;
  padding-bottom: 100px;
  padding-left: 60px;
  padding-right: 60px;
  background-color: #f1f1f1;
  min-height: 500px;
}
#faq-title {
  padding-top: 60px;
  padding-bottom: 60px;
  padding-left: 60px;
  padding-right: 60px;
  font-size: 60px;
}
</style>
