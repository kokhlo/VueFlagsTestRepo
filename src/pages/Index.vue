<template>
  <q-page class="flex flex-center">
    <div class="flex flex-center text-left">
    <p><strong>Country flags (11):</strong></p>
    <div class="fit row wrap justify-center items-center content-start">
      <country-flag
        :rounded="true"
        v-for="(country, index) in countries"
        :key="index"
        :country="country"
        size="big"
      />
    </div>
    <div>
      <div>New ones:</div>
      <br />
      <flag iso="it" />
      <br />
      <flag :squared="true" iso="gb" />
      <br />
      <flag iso="us" style="height: 3.5vh; width: 7.7vw;" />
      <br />
      <flag iso="ua" style="border-radius: 25px; height: 3.5vh; width: 12vw;" />
      <br />
    </div>
  </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
  data() {
    return {
      countries: ['gb', 'fr', 'es', 'it', 'ru', 'pt', 'de', 'pl', 'kr', 'jp', 'cn'],
    };
  },
};
</script>
