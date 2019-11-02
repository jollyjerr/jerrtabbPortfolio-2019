<template>
    <div class="project-listing" >
        <header>
            <a :href="project.link" target="_blank" rel="noopener noreferrer">
            <h2>{{project.name}}</h2>
            </a>
            <a :href="project.link" target="_blank" rel="noopener noreferrer" class="git">
                <i class="fab fa-github"></i>
            </a>
        </header>
        <img :src="project.image" :alt="project.name">
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
.project-listing {
    width: 100%;
    padding: 2%;
    header {
        display: flex;
        justify-content: space-between;
        padding: 0;
        a {
            color: $text;
            margin: auto;
        }
        i {
            font-size: 180%;
        }
        .git {
            display: block;
            width: max-content;
        }
    }
    h2 {
        color: $text;
    }
    a {
        text-decoration: none;
    }
    img {
        width: 100%;
    }
}
</style>