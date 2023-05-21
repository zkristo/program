<script>
export default {
    name: "HomeComponent",
    data() {
        return {
            data: []
        }
    },
}

</script>

<template>
    <body>
        <button type="button">Prethodna ruta</button>
        <button type="button">Sljedeca ruta</button>

        <br>
        <br>
        <form action="/action_page.php">
            <label for="naziv">Naziv</label>
            <input type="text" id="naziv" name="fname"><br><br>
            <label for="admin">Administrator</label>
            <select id="admin" name="admin">
                <option value="admin1">Admin1</option>
                <option value="admin2">Admin2</option>
            </select>
            <br><br>
            <input type="submit" value="Spremi">
            <button type="button">Izbriši</button>
        </form>

        <hr>
        <h1>Stanice</h1>

    </body>
</template>
