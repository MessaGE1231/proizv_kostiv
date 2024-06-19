<button id="btn" value="{val}" on:click={check} class="border-black border-solid border-2 w-4 h-4 rounded-full "></button>


<style lang="postcss">
:global(html) {
    background-color: theme(colors.gray.100);
}
</style>

<script>
import "../routes/style.css";

    $: val = false
    
function check () {
    val == false ? val = true : val = false 
    val == false ? btn.style.background = "white" : btn.style.background = "lightblue"
}
</script>
