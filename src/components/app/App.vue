<template>
  <div class="app">
    <div class="content">
      <AppInfo />
      <div class="search_panel">
        <SearchPanel />
        <AppFilter />
      </div>
      <div>
        <MovieList />
        <MovieAddForm />
      </div>
    </div>
  </div>
</template>

<script>
import AppInfo from "@/components/app_info/AppInfo.vue"
import SearchPanel from "@/components/sear_panel/SearchPanel.vue"
import AppFilter from "@/components/app_filter/AppFilter.vue"
import MovieList from "@/components/movie_list/MovieList.vue"
import MovieAddForm from "@/components/movie_add/MovieAddForm.vue"
export default {
  components: {
    AppInfo,
    SearchPanel,
    AppFilter,
    MovieList,
    MovieAddForm,
  },
}
</script>

<style>
.app {
  height: 100vh;
  color: #000;
}

.content {
  width: 1000px;
  min-height: 700px;
  background-color: #fff;
  margin: 0 auto;
  padding: 5rem 0;
}

.search_panel {
  margin-top: 2rem;
  padding: 1.5rem;
  background-color: #fcfaf5;
  border-radius: 4px;
  box-shadow: 15px 15px 15px 15px rgba(0, 0, 0, 0.15);
}
</style>