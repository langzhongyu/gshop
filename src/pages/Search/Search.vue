<template>
  <div>
    <section class="search">
      <HeaderTop :title="search"></HeaderTop>
      <form class="search_form" action="#">
        <input type="search" name="search" placeholder="请输入商家或美食名称" class="search_input">
        <input type="submit" name="submit" class="search_submit">
      </form>
      <FooterGuide></FooterGuide>
    </section>
  </div>
</template>

<script>
import HeaderTop from '../../components/HeaderTop/HeaderTop.vue'
import FooterGuide from '../../components/FooterGuide/FooterGuide.vue'
export default {
  name: 'search',
  data () {
    return {
      search:'搜索'
    }
  },
  components:{
    HeaderTop,
    FooterGuide
  }
}
</script>

<style scoped>
  .search {
    width: 100%;
  }
  .search .search_form {
    *zoom: 1;
    margin-top: 45px;
    background-color: #fff;
    padding: 12px 8px;
  }
  .search .search_form::after {
    content: '';
    display: block;
    clear: both;
  }
  .search .search_form input {
    height: 35px;
    padding: 0 4px;
    border-radius: 2px;
    font-weight: bold;
    outline: none;
  }
  .search .search_form input.search_input {
    float: left;
    width: 79%;
    border: 4px solid #f2f2f2;
    font-size: 14px;
    color: #333;
    background-color: #f2f2f2;
  }
  .search .search_form input.search_submit {
    float: right;
    width: 18%;
    border: 4px solid #02a774;
    font-size: 16px;
    color: #fff;
    background-color: #02a774;
  }
</style>
