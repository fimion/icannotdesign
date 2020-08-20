<script>
import DefaultLayout from './default.vue';

export default {
  name: 'handrawn',
  extends: DefaultLayout,
  head:{
    link: [
      { rel: 'stylesheet', href: '/css/handrawn.min.css'},
    ]
  }
}
</script>
