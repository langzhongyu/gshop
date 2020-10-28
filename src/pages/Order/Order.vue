<template>
  <div>
    <section class="order">
      <headerTop :title="order">
      </headerTop>
      <section class="order_no_login">
        <img src="../../assets/images/order/person.png">
        <h3>登录后查看外卖订单</h3>
        <button>立即登陆</button>
      </section>
      <FooterGuide></FooterGuide>
    </section>
  </div>
</template>

<script>
import headerTop from '../../components/HeaderTop/HeaderTop.vue'
import FooterGuide from '../../components/FooterGuide/FooterGuide.vue'
export default {
  name: 'order',
  data () {
    return {
      order:'订单列表'
    }
  },
  components:{
    headerTop,
    FooterGuide
  }
}
</script>

<style scoped>
.order {
  width: 100%;
}
.order .order_no_login {
  padding-top: 140px;
  width: 60%;
  margin: 0 auto;
  text-align: center;
}
.order .order_no_login >img {
  display: block;
  width: 100%;
  height: 30%;
}
.order .order_no_login >h3 {
  padding: 10px 0;
  font-size: 17px;
  color: #6a6a6a;
}
.order .order_no_login >button {
  display: inline-block;
  background: #02a774;
  font-size: 14px;
  color: #fff;
  border: 0;
  outline: none;
  border-radius: 5px;
  padding: 10px 20px;
}
</style>
