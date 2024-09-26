<script setup>

</script>

<template>
    <header class="upper">
        <nav>
            <div class="toptext" style="margin-left: 5.5%;">
            <img class="logo" src="@/assets/s3vin-logo.svg"/>
            <p style="font-size: 37.524px; font-weight: 700;">S3V!N</p>
            </div>
            <div class="toptext" style="margin-right: 5.5%;">
            <img class="generalicon" src="@/assets/grid-9-icon.svg"/>
            <img class="generalicon" src="@/assets/bell-icon.svg"/>
            <img class="profile" src="@/assets/pfp-icon.png"/>
            </div>
        </nav>
        <hr style="border: 1px solid #475467;"/>
        <nav>
            <div class="toptext" style="margin-left: 5.5%;">
                <button class="home">App Launcher</button>
            </div>
            <div class="toptext" style="margin-right: 5.5%;">
                <img class="generalicon" src="@/assets/grid-9-icon.svg"/>
                <img class="generalicon" src="@/assets/chevron-right.svg">
                <p style="white-space: nowrap; font-size:14px;">App Launcher</p>
            </div>
        </nav>
    </header>
    <header class="lower">
        <nav>
            <div class="lowertext" style="margin-left:5.5% ;">
                <p style="font-size: 24px;font-weight: 600;">App Launcher</p>
                <p style="font-weight: 400;font-size: 16px;">Launch an app below to supercharge your work day.</p>
            </div>
            <div style="margin-right: 5.5%;">
                <button class="apppermission">+ Request App Permission</button>
            </div>
        </nav>
    </header>
    <header class="middle">
        <div class="list">
            <button class="filters">View All</button>
            <button class="filters">Developer tools</button>
            <button class="filters">For Admins</button>
            <button class="filters">For Business</button>
        </div>
        <div>
        <hr style="width: 89%;"/>
        </div>
    </header>
    <header class="cards">

        <div class="row">
            <div class="col-sm-6 mb-3 mb-sm-0">
                <div class="card">
                <div class="card-body">
                    <h5 class="card-title">Special title treatment</h5>
                    <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                    <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
                </div>
            </div>
            <div class="col-sm-6">
                <div class="card">
                <div class="card-body">
                    <h5 class="card-title">Special title treatment</h5>
                    <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                    <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
                </div>
            </div>
        </div>
        <div class="row">
            <div class="col-sm-6 mb-3 mb-sm-0">
                <div class="card">
                <div class="card-body">
                    <h5 class="card-title">Special title treatment</h5>
                    <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                    <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
                </div>
            </div>
            <div class="col-sm-6">
                <div class="card">
                <div class="card-body">
                    <h5 class="card-title">Special title treatment</h5>
                    <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                    <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
                </div>
            </div>
        </div>

    </header>
    <header class="pagenav">
        <div style="margin:0% 5.5%;">
            <hr />
        </div>
        <nav>
            <div class="pagecont" style="margin-left: 5.5%;">
                <div class="pagenavfont">
                <img src="@\assets\arrow-narrow-left.svg" style="margin-right: 5px;width: 20px;height: 20px;">
                <p class="pagenavfont">Previous</p>
                </div>
            </div>
            <div class="pagecont" style="margin-right: 5.5%;">
                <div class="pagenavfont">
                <p>Next</p>
                <img src="@\assets\arrow-narrow-right.svg" style="margin-left: 5px;width: 20px;height: 20px;">
                </div>
            </div>
        </nav>
    </header>
</template>

<style scoped>

    .upper{
        background-color: #0C111D;
        width: 100%;
        position: fixed;
    }

    .lower{
        color: black;
        margin-top: 184px;
        width: 100%;
        position: fixed;
    }

    .middle{
        margin-top: 275px;
        margin-left: 5.5%;
        width: 100%;
        position: fixed;
    }

    .cards{
        margin-top: 366px;
        margin-left: 5.5%;
        width: 100%;
        position: fixed;
    }

    .card-text{
        color: black;
    }

    .pagenav{
        margin-top: 990px;
        width: 100%;
        position: fixed;

    }

    nav{
        align-items:center;
        display:flex;
        flex-direction: row;
        width:100%;
        justify-content: space-between;
    }

    .pagecont{
        padding-top: 20px;
        display:flex;
        flex-direction: row;
        align-items:center;
    }

    .logo{
        margin-right: 10px;
        height: 39.75px;
        width: 45px;
        background:transparent;
    }

    .generalicon{
        height: 40px;
        padding: 8px;
        border-radius: 10px;

        &:hover{
            background-color: #182230;
            cursor: pointer;
        }
    }

    .profile{
        width:40px;
        height: 40px;
        border-radius: 50px;
        &:hover{
            background-color: #182230;
            cursor: pointer;
        }
    }

    .home{
        color: #FFF;
        font-size: 16px;
        background-color: transparent;
        border-style: none;
        padding: 8px 12px;
        border-radius: 6px;
        &:hover{
            background-color: #182230;
            cursor: pointer;
        }
    }

    .toptext{
        color:#FFF ;
        padding: 12px 0px;
        display:flex;
        flex-direction: row;
        align-items:center;
    }

    .lowertext{
        color:#030712 ;
    }

    .apppermission{
        color: #475467;
        font-weight:600;
        background-color: white;
        font-size: 14px;
        border-radius: 5px;
        padding:10px 14px;
        border: 1px solid #E5E7EB;
        &:hover{
            cursor: pointer;
        }
    }

    .filters{
        color: #667085;
        font-weight: 600;
        font-size: 14px;
        padding-bottom: 12px;
        border-style: none;
        background-color: transparent;
        &:hover{
            color:#059669;
            border-bottom: 2px solid #10B981;
            cursor: pointer;
        }
    }

    .pagenavfont{
        font-size: 14px;
        font-weight: 600;
        color:#475467;
        &:hover{
            cursor: pointer;
        }
        
    }

</style>
