Model View View Model pattern is what we'll be using. For our project.

Other patterns:

MVC
MV*

Always use the composition API for vue. Don't use the options one. Learn the concepts of the composition API.

Using Vue in your html:

<script src="https://unpkg.com/vue@3/dist/vue.global.js"></script>

const { createApp, ref } = Vue

  createApp({
    setup() {
      const message = ref('Hello vue!')
      return {
        message
      }
    }
  }).mount('#app')


In javascript, try using const first. If you can't use const, use let, and if you can't use let, use var.

  Const

  Let

  Var


Homework: Make a to do list. Upload project to render.
