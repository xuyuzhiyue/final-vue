<template>
  <div class="wrapper" ref="aaaa">
    <ul class="content">
      <li>haha1</li>
      <li>haha2</li>
      <li>haha3</li>
      <li>haha4</li>
      <li>haha5</li>
      <li>haha6</li>
      <li>haha7</li>
      <li>haha8</li>
      <li>haha9</li>
      <li>haha10</li>
      <li>haha11</li>
      <li>haha12</li>
      <li>haha13</li>
      <li>haha14</li>
      <li>haha15</li>
      <li>haha16</li>
      <li>haha17</li>
      <li>haha18</li>
      <li>haha19</li>
      <li>haha20</li>
      <li>haha21</li>
      <li>haha22</li>
      <li>haha23</li>
      <li>haha24</li>
      <li>haha25</li>
      <li>haha26</li>
      <li>haha27</li>
      <li>haha28</li>
      <li>haha29</li>
      <li>haha30</li>
      <li>haha31</li>
      <li>haha32</li>
      <li>haha33</li>
      <li>haha34</li>
      <li>haha35</li>
      <li>haha36</li>
      <li>haha37</li>
      <li>haha38</li>
      <li>haha39</li>
      <li>haha40</li>
      <li>haha41</li>
      <li>haha42</li>
      <li>haha43</li>
      <li>haha44</li>
      <li>haha45</li>
      <li>haha46</li>
      <li>haha47</li>
      <li>haha48</li>
      <li>haha49</li>
      <li>haha50</li>
      <li>haha51</li>
      <li>haha52</li>
      <li>haha53</li>
      <li>haha54</li>
      <li>haha55</li>
      <li>haha56</li>
      <li>haha57</li>
      <li>haha58</li>
      <li>haha59</li>
      <li>haha60</li>
      <li>haha61</li>
      <li>haha62</li>
      <li>haha63</li>
      <li>haha64</li>
      <li>haha65</li>
      <li>haha66</li>
      <li>haha67</li>
      <li>haha68</li>
      <li>haha69</li>
      <li>haha70</li>
      <li>haha71</li>
      <li>haha72</li>
      <li>haha73</li>
      <li>haha74</li>
      <li>haha75</li>
      <li>haha76</li>
      <li>haha77</li>
      <li>haha78</li>
      <li>haha79</li>
      <li>haha80</li>
      <li>haha81</li>
      <li>haha82</li>
      <li>haha83</li>
      <li>haha84</li>
      <li>haha85</li>
      <li>haha86</li>
      <li>haha87</li>
      <li>haha88</li>
      <li>haha89</li>
      <li>haha90</li>
      <li>haha91</li>
      <li>haha92</li>
      <li>haha93</li>
      <li>haha94</li>
      <li>haha95</li>
      <li>haha96</li>
      <li>haha97</li>
      <li>haha98</li>
      <li>haha99</li>
      <li>haha100</li>
    </ul>
  </div>
</template>

<script>
  import BScroll from 'better-scroll'
  export default {
    name: "Category",
    data(){
      return{
        scroll:null
      }
    },
    mounted() {
      console.log(this.$refs.aaaa);
      console.log(document.querySelector('.wrapper'));
      this.scroll =new BScroll(document.querySelector('.wrapper'),{
        // 监听所有属性
        probeType:3,
        pullUpLoad:true
      })

      this.scroll.on('scroll',(position)=>{
        console.log(position);
      })
      this.scroll.on('pullingUp',()=>{
        console.log('上拉下载更多');
      })
    }
    // 组件创建完成
    // created() {
    //   new BScroll('.content',{
    //
    //   })
    // }
  }
</script>

<style scoped>
  .wrapper{
    height: 100px;
    background-color: salmon;
    overflow: hidden;
    /*overflow-y: scroll;*/
  }
</style>
