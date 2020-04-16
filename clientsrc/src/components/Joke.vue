<template>
<b-col cols="3" class="m-1">
<b-card
        border-variant="success"
        :header="jokeData.setup"
        header-bg-variant="success"
        header-text-variant="white"
        header-tag="header"
        align="center"
        class="jokeCards"
      >
        <b-card-text>
          <p>{{jokeData.punchline}}</p>
    <p>Created by: {{jokeData.creator.name}}</p>
    </b-card-text>
      </b-card>
</b-col>
</template>


<script>
export default {
  name: "joke",
  props: ["jokeData"],
  data() {
    return {};
  },
  computed: {},
  methods: {},
  components: {}
};
</script>


<style scoped>
.jokeCards {
  height: 13rem;
}
header {
  height: 65px;
}
</style>