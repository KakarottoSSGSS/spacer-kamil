<template>
      
      
      <input id="search"
             name="search"
             :class="{ dark: dark }"
             :value="value"
             @input="handleChange"
      >
      
</template>

<script>
export default {
    name: SearchInput,
    props: {
      value: {
        type: String,
        required: true,
      },
      dark: {
        type: Boolean,
        default: false,
      }
    },
    methods: {
      // emituje vartos zmiennej do rodzica
      handleChange(e) {
        this.$emit('input',e.target.value)
      }
    }
};
</script>

<style lang="scss" scoped>

input {
  margin-top: 50px;
  display: flex;
  width: 250px;
  color: white;
  text-align: center;
  font-size: 30px;
  font-weight: 300;
  height: 30px;
  border: 0;
  border-bottom:  1px solid white;
  background: none;
  transition:  box-shadow .3s ease-in-out;

   @media (min-width: 1024px) {
    font-weight: 400;

  }
}

input:focus {
  box-shadow: 0 10px 20px -8px rgba(255,255,255,.6);
  outline: none;
}

.dark {
  color:#1e3d4a;;
  border-bottom-color:#1e3d4a;
}

.dark:focus {
  box-shadow: 0 10px 20px -8px rgba(#1e3d4a,.6);
}
</style>
