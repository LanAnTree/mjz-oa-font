<template>
  <div>
    <div>账号切换</div>
    <button @click="zhangsan()" type="default" size="mini">张三</button>
    <button @click="lisi()" type="default" size="mini">李四</button>
    <button @click="zzjl()" type="default" size="mini">张总经理</button>
    <button @click="admin()" type="default" size="mini">admin</button>
    <div>当前token：{{ token }}</div>
  </div>
</template>

<script>
export default {
  name: "Test",

  data() {
    return {
      token: ''
    };
  },

  created(){
    this.token = window.localStorage.getItem('token')
  },

  methods: {
    admin() {
      window.localStorage.setItem('mjz_oa_token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDewtDQ3MTI10VEqLU4t8kwBikGYeYm5qUAtiSm5mXlKtQAI_i11QgAAAA.AnghnD5dJqunfk8WSWU6itIXmztuPoYYnYrGdgBovE_l0MQx2vBUHJqVXHiqcF6sUrE-AoxbMEj11-ki-H6JWQ'
      window.localStorage.setItem('mjz_oa_token', token);
      this.token = window.localStorage.getItem('mjz_oa_token')
    },

    zhangsan() {
      window.localStorage.setItem('mjz_oa_token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDewtDQ3MTQ111EqLU4t8kxRsoIy8xJzU4FaqjIS89KLE_OUagFlG7MHRQAAAA.TEID4kng-v9_KP3j8uupwomnE3LJ1RlGTrC2FrXmEtUk1YYn__qIApRWPhGYqALzl-HXWSY6SxhgltwXkx4P1w'
      window.localStorage.setItem('mjz_oa_token', token);
      this.token = window.localStorage.getItem('mjz_oa_token')
    },

    zzjl() {
      window.localStorage.setItem('token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDewtDQ3MjG30FEqLU4t8kxRsjKDMPMSc1OBWhJTcjPzlGoBD-tr9EIAAAA.LIPL3Bf85OjC-ds-YPYA9BsSLoQ9XxV7oJd50uupR_pUQCeZtaOoW-B7Myhx-oaPrD6LAFfdpi9HmgdZgXGrbw'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    },

    lisi() {
      window.localStorage.setItem('mjz_oa_token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDewtDQ3MTIw1VEqLU4t8kxRsjKBMPMSc1OBWnIyizOVagF4eNq-QQAAAA._hU7sg1KjlgHmRLDZexcyopCFOCAMYo9WOPDNcx7n3m6Hwbo1f0rAxs_zq91kMSghe6fiUVzzQVkwVmtExa2hQ'
      window.localStorage.setItem('mjz_oa_token', token);
      this.token = window.localStorage.getItem('mjz_oa_token')
    }
  }
}
</script>
