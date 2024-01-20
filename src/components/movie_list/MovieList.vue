<template>
    <ul class="movie-list list-group">
    <MovieListItem v-for="movie in movies" />
    </ul>
</template>

<script>
import MovieListItem from "@/components/movie_list_item/MovieListItem.vue";

export default {
    components: { MovieListItem },
    data() {
        return {
            movies: [
                {
                    name: "Movie 1",
                    viewers: 345
                },
                {
                    name: "Movie 2",
                    viewers: 332
                },
                {
                    name: "Movie 3",
                    viewers: 988
                }
            ]
        }
    }
}
</script>

<style scoped>
.movie-list {
    margin-top: 2rem;
    padding: 1.5rem;
    background-color: #fcfaf5;
    border-radius: 4px;
    box-shadow: 15px 15px 15px 15px rgba(0, 0, 0, 0.15);
}
</style>