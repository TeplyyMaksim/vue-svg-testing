<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>I present to you my beautiful icons</h2>
    <ul>
      <li class="initial">My Backarrow <svgicon name="back-arrow"  height="1.5em" width="auto" color="#42b983 #35495e"></svgicon></li>
      <li>
        My copier
        <svgicon
          name="copier"
          height="5em"
          width="auto"
          color="#42b983 #35495e #333333 #fff000 #ff00ff #ffffff" />
      </li>
      <li>Transfer <svgicon name="transfer"  height="1.5em" width="auto" color="#888222" dir="up"></svgicon></li>
      <li class="nameless">Eraser <svgicon name="eraser"  height="2em" width="auto" :fill="false" ></svgicon></li>
      <li class="afternoon">Gradient target <svgicon name="target"  height="2em" width="auto" color="url(#gradient-1) url(#gradient-2)"></svgicon></li>
    </ul>
    <svg>
       <defs>
          <linearGradient id="gradient-1" x1="0" y1="0" x2="0" y2="1">
              <stop offset="5%"  stop-color="#57f0c2"/>
              <stop offset="95%" stop-color="#147d58"/>
          </linearGradient>
          <linearGradient id="gradient-2" x1="0" y1="0" x2="0" y2="1">
              <stop offset="5%"  stop-color="#7295c2"/>
              <stop offset="95%" stop-color="#252e3d"/>
          </linearGradient>
      </defs>
    </svg>
  </div>
</template>

<script>
import './icons/back-arrow';
import './icons/copier';
import './icons/eraser';
import './icons/target';
import './icons/transfer';

export default {
  name: 'IconComponent',
  data() {
    return {
      msg: 'Welcome to the jungle!',
    };
  },
};
</script>

<style lang="scss" scoped>
h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;

  li {
    display: inline-block;
    margin: 0 1em;
  }
}
</style>
