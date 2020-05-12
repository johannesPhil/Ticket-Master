<template>
    <header>
        <div class="logo"><h1>LOGO</h1></div>
        <div class="headerlinks">
            <a href="" class="headerlinks__getticket headerlinks--nobg">
                I didn't get my tickets
            </a>
            <a href="" class="headerlinks__createevent headerlinks--bg">
                create your own event
            </a>
        </div>
    </header>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
header{
    max-width: 90%;
    display:flex;
    flex-direction: row;
    justify-content: space-between;
}
.headerlinks{
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
}
.headerlinks--nobg{
    color: #000;
}
.headerlinks--bg{
border-radius: 4.06693px;
}
</style>