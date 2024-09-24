<script setup>

</script>

<template>
    <header class="upperhead">
        <nav>
            <img class="logo" src="@/assets/s3vin-logo.svg"/>
            <p style="font-size: 37.524px;">S3V!N</p>
            <img class="grid-upper" style="margin-left: 72%;" src="@/assets/grid-9-icon.svg"/>
            <img class="bell" src="@/assets/bell-icon.svg"/>
            <img class="profile" src="@/assets/pfp-icon.png"/>
        </nav>
        <hr style="border: 1px solid #475467;"/>
        <nav>
            <p style="padding: 8px 12px;white-space: nowrap;background-color: #182230;border-radius: 10px;">App Launcher</p>
            <img class="grid-lower" style="margin-left: 72.5%;" src="@/assets/grid-9-icon.svg"/>
            <img class="chevron" src="@/assets/chevron-right.svg">
            <p style="white-space: nowrap; font-size:14px;">App Launcher</p>
        </nav>
    </header>
</template>

<style scoped>

    .upperhead{
        background-color: #0C111D;
        z-index: 99;
        width: 100%;
        position: fixed;
    }

    nav{
        display:flex;
        flex-direction: row;
        padding: 10px 0;
        width:100%;
        margin: 0% 7.8%;
    }

    img{
        margin-right: 5px;
    }

    .logo{
        margin-right: 10px;
        margin-top: 10px;
        height: 39.75px;
        width: 45px;
        background:transparent;
    }

    .grid-upper{
        margin-top: 15px;
        height: 30px;
        padding: 6px;
        background-color: #182230;
        border-radius: 10px
    }

    .bell{
        margin-left: 5px;
        margin-right: 15px;
    }

    .grid-lower{
        margin-top: 5px;
        height: 30px;
        padding: 6px;
    }

    .chevron{
        margin-top: 10px;
        width: 20px;
        height: 20px;
        padding: 2px;
    }

    .profile{
        margin-top: 15px;
        width:30px;
        height: 30px;
    }

    p{
        color: white;
       align-content: center;
    }

</style>