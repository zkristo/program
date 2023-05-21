<script>
export default {
    name: "Stanice",
    props: {
        rute: Object
    }
}
</script>

<template>
    <h3># Naziv stanice</h3>
    <div v-for="stanica in rute[0].stanice">
        <h3>{{ stanica }}</h3>
    </div>
</template>