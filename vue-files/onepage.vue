<script setup>
import { ref } from 'vue';

const count=ref(0)

</script>

<template>
<body>
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

    <header class="layout-cards">

            <div class="outerborder">
                <div class="inner">
                    <div class="maintitle">
                        <div style="display: flex;flex-direction: row;align-items: center;">
                            <img class="card-icon" src="@/assets/business-icon.svg" style="background-color: rgba(41, 156, 219, 0.10);"/>
                            <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Manage Business</p>
                        </div>
                        <p class="newnote" v-if="count > 0">{{ count }} New</p>
                        <p v-else></p>
                    </div>
                    <p>Assign application access to businesses at a Super Admin level.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button class="card-button">Launch</button>
            </div>

            <div class="outerborder">
                <div class="inner">
                    <div class="maintitle">
                        <div style="display: flex;flex-direction: row;align-items: center;">
                        <img class="card-icon" src="@/assets/manage-account-icon.svg" style="background-color: #FFFBEB;"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Manage User</p>
                        </div>
                        <p class="newnote" v-if="count > 0">{{ count }} New</p>
                        <p v-else></p>
                    </div>
                    <p>Create and manage your user all from a single dashboard.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button class="card-button">Launch</button>
            </div>

            <div class="outerborder">
                <div class="inner">
                    <div class="maintitle">
                        <div style="display: flex;flex-direction: row;align-items: center;">
                        <img class="card-icon" src="@/assets/printer-icon.svg" style="background-color: #ECFDF5;"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Check Printing</p>
                        </div>
                        <p class="newnote" v-if="count > 0">{{ count }} New</p>
                        <p v-else></p>
                    </div>
                        <p>Streamline employee check management for timely payroll distribution</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button class="card-button">Launch</button>
            </div>

            <div class="outerborder">
                <div class="inner">
                    <div class="maintitle">
                        <div style="display: flex;flex-direction: row;align-items: center;">
                        <img class="card-icon" src="@/assets/rubric-icon.svg" style="background-color: #FEF2F2;"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Spread It</p>
                        </div>
                        <p class="newnote" v-if="count > 0">{{ count }} New</p>
                        <p v-else></p>
                    </div>
                    <p>Streamline your workflow with our easy-to-use spreadsheet tool.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button class="card-button">Launch</button>
            </div>

            <div class="outerborder">
                <div class="inner">
                    <div class="maintitle">
                    <div style="display: flex;flex-direction: row;align-items: center;">
                        <img class="card-icon" src="@/assets/accounting-icon.svg" style="background-color: #ECFDF5;;"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Accounting</p>
                    </div>
                        <p class="newnote" v-if="count > 0">{{ count }} New</p>
                        <p v-else></p>
                    </div>
                    <p>Track and manage paid and received invoices.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button class="card-button">Launch</button>
            </div>

            <div class="outerborder">
                <div class="inner">
                    <div class="maintitle">
                        <div style="display: flex;flex-direction: row;align-items: center;">
                        <img class="card-icon" src="@/assets/upload-icon.svg" style="background-color: rgba(75, 56, 179, 0.10);"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">File Uploader</p>
                    </div>
                        <p class="newnote" v-if="count > 0">{{ count }} New</p>
                        <p v-else></p>
                    </div>
                    <p>Keep track of all funded payroll invoices.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button class="card-button">Launch</button>
            </div>

            <div class="outerborder">
                <div class="inner">
                    <div class="maintitle">
                        <div style="display: flex;flex-direction: row;align-items: center;">
                            <img class="card-icon" src="@/assets/zendesk.svg"/>
                            <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Payments Recieved</p>
                        </div>
                            <p class="newnote" v-if="count > 0">{{ count }} New</p>
                            <p v-else></p>
                        </div>
                    <p>Manage and confirmed all recorded payroll payments from customers.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button class="card-button">Launch</button>
            </div>

            <div class="outerborder">
                <div class="inner">
                    <div class="maintitle">
                    <div style="display: flex;flex-direction: row;align-items: center;">
                        <img class="card-icon" src="@/assets/jira.svg"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Groups</p>
                    </div>
                            <p class="newnote" v-if="count > 0">{{ count }} New</p>
                            <p v-else></p>
                    </div>
                    <p>Create, share and save groups that are referenced frequently within the S3V!N system.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button class="card-button">Launch</button>
            </div>

            <div class="outerborder">
                <div class="inner">
                    <div class="maintitle">
                    <div style="display: flex;flex-direction: row;align-items: center;">
                        <img class="card-icon" src="@/assets/dropbox.svg"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Reports</p>
                    </div>
                            <p class="newnote" v-if="count > 0">{{ count }} New</p>
                            <p v-else></p>
                    </div>
                    <p>Generate and download reports custom reports.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button class="card-button">Launch</button>
            </div>
    </header>
    <header class="pagenav">
        <div>
            <hr />
        </div>
        <nav>
            <div class="pagecont">
                <div class="pagenavfont">
                <img src="@\assets\arrow-narrow-left.svg" style="margin-right: 5px;width: 20px;height: 20px;">
                <p class="pagenavfont">Previous</p>
                </div>
            </div>
            <div class="pagecont">
                <div class="pagenavfont">
                <p class="pagenavfont">Next</p>
                <img src="@\assets\arrow-narrow-right.svg" style="margin-left: 5px;width: 20px;height: 20px;">
                </div>
            </div>
        </nav>
    </header>
</body>
</template>

<style scoped>

body{
    min-width: 100vw;
}
    .upper{
        background-color: #0C111D;
        width: 100%;
    }

    .lower{
        color: black;
        margin-top: 32px;
        width: 100%;
    }

    .middle{
        margin-top: 24px;
        margin-left: 5.5%;
        width: 100%;
    }

    .layout-cards{
        margin-left: 5.5%;
        width: 89%;
        margin-top: 24px;
        display:flex;
        flex-direction: row;
        flex-wrap: wrap;
        justify-content: space-evenly;
    }

    .pagenav{
        margin:0% 5.5%;
        margin-top: 24px;
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
        align-items:center;
        display:flex;
        flex-direction: row;
        font-size: 14px;
        font-weight: 600;
        color:#475467;
        &:hover{
            cursor: pointer;
        }
    }

.outerborder{
    font-weight: bold;
    background-color: white;
    border-radius: 10px;
    margin: 0.5% 2%;
    border: 2px solid #E5E7EB;
}

.inner{
    margin:15px;
    color: black;
}

.maintitle{
    display: flex;
    flex-direction: row;
    align-items: center;
    margin-bottom: 10px;
    justify-content: space-between;
}

.card-button{
    width: 180%;
    align-content: end;
    font-weight: bold;
    font-size: 14px;
    border: none;
    padding: 0px;
    background-color: transparent;
    &:hover{
        cursor: pointer;
    }
}

.newnote{
    color:#DC2626;
    margin-bottom: 15px;
    padding: 1px 7px;
    background-color: #FEF2F2;
    border-radius: 20px;
    font-weight: 600;
}

.card-icon{
    border-radius: 5px;
    padding: 5px;
    width: 40px;
}

</style>
