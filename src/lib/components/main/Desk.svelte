<script>
  import DecorBox from "./DecorBox.svelte";

</script>

<div class="desk">
    <div class="on-desk">
        <DecorBox />
        <DecorBox />
        <DecorBox />
        <DecorBox />
        <DecorBox contains=1 />
        <DecorBox />
        <DecorBox />
        <DecorBox />
        <DecorBox />
    </div>
</div>

<style>
    .desk {
        height: 100%;
        width: 100%;
        background-color: rgb(70, 43, 19);
    }

    .on-desk {
        display: grid;
        grid-template-columns: repeat(3, minmax(0, 1fr));
        height: 100vh;
    }
</style>