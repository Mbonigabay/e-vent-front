<template>
    <Layout>
        <h1>{{$page.event.name}}</h1>
    </Layout>
</template>

<page-query>
query {
  event(id:"1") {
    id
    name
    duration
    price
    date
  }
}
</page-query>

<script>
export default {
    metaInfo() {
        return {
            title: this.$page.event.title
        }
    }
}
</script>