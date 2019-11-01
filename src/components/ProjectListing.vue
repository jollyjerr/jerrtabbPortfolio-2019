<template>
    <div class="project-listing" >
        <img :src="project.image" :alt="project.name">
        <a :href="project.link" target="_blank" rel="noopener noreferrer">
            <h3>{{project.name}}</h3>
        </a>
        <p>{{project.description}}</p>
    </div>
</template>

<script>
export default {
    props: {
        project: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/variables.scss';
</style>