<template>
  <div class="col-full">
    <h1>Welcome to the Forum</h1>
    <ThreadList :threads="thread" />
  </div>
</template>
<script>
import sourceData from '@/data'
import ThreadList from '@/components/ThreadList'

export default {
  name: 'PageHome',
  components: { ThreadList },
  data () {
    return {
      thread: Object.values(sourceData.threads),
      posts: sourceData.posts,
      users: sourceData.users
    }
  }
}
</script>