<template>
  <div class="story">
    <span class="score">{{ story.data.score }}</span>
    <router-link :to="{ path: '/story/' + story.data.id }">{{ story.data.title }}</router-link>
    <router-link class="router-link" :to="{ path: '/story/'}"> <span>{{ story.data.url | host }}</span> </router-link>
    <span class="meta">
          by {{ story.data.by }} | {{ story.data.time }} Ago | {{ story.data.descendants }} comments
    </span>
  </div>
</template>

<script>
export default {
  name: 'Item',
  props: [
    'story'
  ]
}
</script>

<style scoped>
.story {
  display: flex;
  flex-direction: column;
  background-color: #fff;
  padding: 20px 30px 20px 80px;
  border-bottom: 1px solid #006d77;
  border-left: 10px solid #006d77;
  box-shadow: 10px 5px 5px #1414147c;
  border-radius: 10px;
  position: relative;
  line-height: 20px;
  margin: 10px;
  text-align: justify;
}
.story:hover{
  -moz-transform: scale(1.05);
	-webkit-transform: scale(1.05);
	transform: scale(1.05);
}
.score{
  color: #006d77;
  font-size: 1.1em;
  font-weight: 700;
  position: absolute;
  top: 50%;
  left: 0;
  width: 80px;
  text-align: center;
  margin-top: -10px;
}
.story a {
  color: #34495e;
  font-weight: 600;
  text-decoration: none;
}
.story a span {
  font-size: .85em;
  margin-left: 10px;
  color: #828282;
}
.story .meta {
  font-size: .85em;
  color: #828282;
  margin: 0 10px;
}

.router-link span {
  word-wrap: break-word;
}
</style>