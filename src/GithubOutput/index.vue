<!-- src/GithubOutput/index.vue-->
<template>
    <div>
 <!-- src/GithubOutput/index.vue -->
<p v-if="currentUsername == null">
  Enter a username above to see their GitHub data
</p>
<p v-else>
  Below are the results for {{ currentUsername }}
  <div v-if="githubData[currentUsername]">
    <h4>{{ githubData[currentUsername].name }}</h4>
    <p>{{ githubData[currentUsername].company }}</p>
    <p>Number of repos: {{ githubData[currentUsername].public_repos }}</p>
  </div>
</p>
    </div>
</template>

<script src="./script.js"></script>
<style scoped src="./style.css"></style>