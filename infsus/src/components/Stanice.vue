<template>
    <div v-for="stanica in stanice">
        <h3>{{ stanica }}</h3>

    </div>
</template>

<script>
export default {
    name: "Stanice",
    props: {
        stanice: Array
    }
}
</script>