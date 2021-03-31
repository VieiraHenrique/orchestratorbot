<template>
  <div class="benefits">
    <div class="container">
      <h2>Benefits for your <span>business</span></h2>
      <div class="benefits__cards">
        <div class="card" v-for="card in cards" :key="card.id">
          <img :src="require(`~/assets/img/${card.img}`)" :alt="card.title" />
          <h3>{{ card.title }}</h3>
          <p>
            {{ card.text }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cards: [
        {
          img: 'easy.png',
          title: 'Easy',
          text: `OrchestratorBot for JD Edwards is the easiest way possible to make
            your orchestrations and notifications instantly available in your
            favorite team collaboration tools and accessible for your entire
            organization with just a few clicks and without a single line of
            code.`,
        },
        {
          img: 'powerful.png',
          title: 'Powerful',
          text: `Finally automate repetitive business tasks with quick actions, define your own user specific templates, bring workflows alive in the team collaboration hub, execute any available orchestration with dynamic forms and instantly upload files into JD Edwards.`,
        },
        {
          img: 'mobile.png',
          title: 'Mobile',
          text: `Mobility is key! Using OrchestratorBot brings you the added value of the MS Teams mobile app. Communicate, collaborate, meet, share and increase productivity right from your own mobile device. Anytime. Anywhere. Deliver any task and business process to your mobile workforce with ease.`,
        },
        {
          img: 'secure.png',
          title: 'Secure',
          text: `Leverage both the enterprise-grade MS Teams privacy, security and compliance as well as native JD Edwards security on the User Defined Objects (UDO). Let your company admin distribute the functionality on a per user basis. `,
        },
      ],
      cardsTwo: [
        {
          img: 'easy.png',
          title: 'TEAMS AGILITY',
          text: `Focus on productivity and team collaboration to spark innovation, enable agility and deliver better results.`,
        },
        {
          img: 'powerful.png',
          title: 'EMBEDDED AI/ML',
          text: `Use the latest best-of-breed technology to seamlessly include AI/ML to improve the effectiveness of your workforce.`,
        },
        {
          img: 'mobile.png',
          title: 'ACTIONABLE INTELLIGENCE',
          text: `Transform your static system of records into an actionable and intelligent system of actions for powerful engagements.`,
        },
        {
          img: 'secure.png',
          title: 'AUTOMATE AND SIMPLIFY',
          text: `Simplification is the main outcome of automation. Reduce complexity and errors in your business processes and simplify routine tasks.`,
        },
        {
          img: 'secure.png',
          title: 'WORKING EVERYWHERE',
          text: `The modern workforce needs a reliable way to work from any location, on any device at any time using a single, secure and intelligent digital workspace.`,
        },
      ],
    }
  },
}
</script>

<style></style>
