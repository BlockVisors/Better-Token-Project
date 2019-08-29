<template>
  <div id="container">
    <h2 id="cause-tit">Top Causes</h2>
    <b-card-group deck>
      <b-card
        id="indiv-card"
        title="Title"
        img-src="https://picsum.photos/300/300/?image=41"
        img-alt="Image"
        img-top
      >
        <b-card-text>
          This is a wider card with supporting text below as a natural lead-in
          to additional content. This content is a little bit longer.
        </b-card-text>
        <div slot="footer">
          <small class="text-muted">Last updated 3 mins ago</small>
        </div>
      </b-card>

      <b-card
        title="Mom's Dental"
        img-src="https://picsum.photos/300/300/?image=41"
        img-alt="Image"
        img-top
      >
        <b-card-text>
          This card has supporting text below as a natural lead-in to additional
          content.
        </b-card-text>
        <div slot="footer">
          <small class="text-muted">Last updated 30 mins ago</small>
        </div>
      </b-card>

      <b-card
        title="Title"
        img-src="https://picsum.photos/300/300/?image=41"
        img-alt="Image"
        img-top
      >
        <b-card-text>
          This is a wider card with supporting text below as a natural lead-in
          to additional content. This card has even longer content than the
          first to show that equal height action.
        </b-card-text>
        <div slot="footer">
          <small class="text-muted">Last updated 3 mins ago</small>
        </div>
      </b-card>
    </b-card-group>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
  methods: {
    onClick() {}
  }
}
</script>
<style scoped>
#container {
  padding: 85px 85px;
  background-color: #35495e;
}
#indiv-card {
  box-shadow: 4px;
  border-radius: 0px;
}
#cause-tit {
  margin-bottom: 40px;
  color: white;
  font: Avenir;
}
</style>
