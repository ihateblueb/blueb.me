<script>
    function partyMode() {
        console.log("EE!EE!")
        console.log("EE!!!!EEeee!!!EEE!")
        console.log("EEE!!!EeEEe!")
    }
</script>

<div class="footer">
    <div>
         &copy; 2022-2023 ihateblueb
         <!-- &bull; <a on:click={partyMode}>party mode</a> -->
    </div>
</div>

<style>
    .footer {
        color: var(--txt1);
        display: flex;

        & a {
            cursor: pointer;
            transition: 0.1s;
        }
        & a:hover {
            color: var(--accent1);
        }
    }
</style>