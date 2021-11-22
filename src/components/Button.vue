<template>
  <div>
      <button :class="btnStyle" >{{ buttonText }}</button>
  </div>
</template>

<script>
export default {
    name: 'Button',
    props: ['buttonText', 'btnStyle']
}
</script>

<style>
.swal2-styled.swal2-confirm {
    border: 0;
    border-radius: 0.25em;
    background: initial;
    background-color: #F29091;
    color: #fff;
    font-size: 1.0625em;
}
</style>