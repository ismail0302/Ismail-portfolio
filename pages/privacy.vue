<template>
  <div class="container mx-auto px-4 my-8 min-h-screen bg-gray-100 prose">
    <h1>
      Privacy Policy
    </h1>
    <p>
      Hey you! First of all, thanks for your interest in my privacy policy.<br>
      I deeply care about the security of your data and will do my best to collect only the needed information and
      protect those!
    </p>

    <h2>
      Overview
    </h2>

    <h3>
      Who is responsible for the collection of data?
    </h3>
    <p>
      That's me, or better said my company: Development. Our contact data can be found in the
      <NuxtLink
        to="/legal/"
        rel="nofollow"
        v-text="'legal notice'"
      />.
    </p>

    <h3>
      How do we collect your data?
    </h3>
    <p>
      We collect data you provide us when you contact us (eg. through the contact form, e-mail, telephone or social
      media).<br>
      Furthermore we collect data anonymized through Google Analytics (see 3.). We do not collect any personal
      data.<br>
      Technical data (like the OS, screen size, language preference, browser) is collected automatically to improve your
      website experience.
    </p>

    <h3>
      How do we use your data?
    </h3>
    <p>
      We use statistics to further develop the Website, to recognize problems or errors and to find out what you, the
      user, like most.
    </p>

    <h3>
      What are your rights?
    </h3>
    <p>
      You have the right to request information about purpose, origin and recipients of your data at any given time and
      free of charge.<br>
      You can demand correction, locking or deletion of your data.<br>
      Also you can revoke given consents for processing data. <br>
      To file a request, simply send a mail to mi477048@gmail.com<br>
      But as we don't save any personal data, we will likely tell you that we don't have any data
      about you.<br>
      <br>
      In case we don’t comply with your request, you have the right to complain at the responsible regulating authority.<br>
      Of course, it’s in our interest to guarantee your personal data privacy.<br>
      If you have any questions please feel free to contact us via 18mdswe013@uetmardan.edu.pk<br>
    </p>
  </div>
</template>

<script>
export default {
  head () {
    return {
      title: 'Privacy - Lichter.io',
      meta: [
        { hid: 'robots', name: 'robots', content: 'noindex' }
      ]
    }
  },
  methods: {
    optOut () {
      document.cookie = 'ga_optout=true; expires=Thu, 31 Dec 2099 23:59:59 UTC; path=/'
      this.$ga.disable()
    }
  }
}
</script>
