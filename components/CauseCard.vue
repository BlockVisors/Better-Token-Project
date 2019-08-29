<template>
  <div>
    <b-card id="container">
      <b-media no-body>
        <b-media-aside vertical-align="center">
          <b-img
            blank
            blank-color="#ccc"
            width="128"
            height="256"
            alt="placeholder"
          ></b-img>
        </b-media-aside>

        <b-media-body class="ml-3">
          <h5 class="mt-0">Media Title</h5>
          <p>
            Cras sit amet nibh libero, in gravida nulla. Nulla vel metus
            scelerisque ante sollicitudin. Cras purus odio, vestibulum in
            vulputate at, tempus viverra turpis. Fusce condimentum nunc ac nisi
            vulputate fringilla. Donec lacinia congue felis in faucibus.
          </p>
          <p class="mb-0">
            Donec sed odio dui. Nullam quis risus eget urna mollis ornare vel eu
            leo. Cum sociis natoque penatibus et magnis dis parturient montes,
            nascetur ridiculus mus.
          </p>

          <b-media>
            <b-img
              slot="aside"
              blank
              blank-color="#ccc"
              width="64"
              alt="placeholder"
            ></b-img>
            <h5 class="mt-0">Nested Media</h5>
            Fusce condimentum nunc ac nisi vulputate fringilla. Donec lacinia
            congue felis in faucibus.
          </b-media>
        </b-media-body>
      </b-media>
    </b-card>
  </div>
</template>

<script>
export default {
  name: 'Causes',
  props: {
    features: {
      type: Array,
      required: true
    }
  }
}
</script>

<style>
#container {
  border-inline-end: 2px;
}
</style>
