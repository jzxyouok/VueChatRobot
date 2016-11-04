<template>
  <div>
    <input type="text" v-model="req" />
    <br />
    <div>
      {{resp}}
      <a v-if="url" :href="url">查看</a>
    </div>
    <br />
    <button v-on:click="send">send</button>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      req: '你好',
      resp: null,
      url: null
    }
  },
  methods: {
    send: function() {
      this.$http.post(
        'http://www.tuling123.com/openapi/api',
        {
          key: 'bd0481fbe8104828af364ad26e67c9de',
          info: this.req,
          userid: 'justsoso'
        }
      ).then(
        (response) => {
          return response.json();
        }
      ).then((json) => {
        this.setData(json);
      });
    },
    setData(json) {
      this.resp = json.text;
      
      if(json.code === 200000) {
          this.url = json.url
      }
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
