<script setup>
import { ref } from 'vue';

const count = ref(0)
const admins = ref(true)
const devtools = ref(true)
const business = ref(true)

function filterViewAll(){
    admins.value = true
    devtools.value = true
    business.value = true
}

function filterAdmins(){
    devtools.value = false
    business.value = false
    admins.value = true
}

function filterBusiness(){
    admins.value = false
    devtools.value = false
    business.value = true
}

function filterDevtools(){
    admins.value = false
    devtools.value = true
    business.value = false
}

</script>

<template>

    <body>
        <header class="upper">
            <nav>
                <div class="toptext" style="margin-left: 5.5%;">
                    <img class="logo" src="@/assets/s3vin-logo.svg" />
                    <p style="font-size: 37.524px; font-weight: 700; margin-top: 15PX;">S3V!N</p>
                </div>
                <div class="toptext" style="margin-right: 5.5%;">
                    <img class="generalicon" src="@/assets/grid-9-icon.svg" />
                    <img class="generalicon" src="@/assets/bell-icon.svg" />
                    <img class="profile" src="@/assets/pfp-icon.png" />
                </div>
            </nav>
            <hr style="border: 1px solid #475467;margin: 0px;" />
            <nav>
                <div class="toptext" style="margin-left: 5.5%;">
                    <button class="home">App Launcher</button>
                </div>
                <div class="toptext" style="margin-right: 5.5%;">
                    <img class="generalicon" src="@/assets/grid-9-icon.svg" />
                    <img class="generalicon" src="@/assets/chevron-right.svg">
                    <p style="white-space: nowrap; font-size:14px; margin-top: 15px;">App Launcher</p>
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
            <div>
                <button class="filters" @click="filterViewAll">View All</button>
                <button class="filters" @click="filterDevtools">Developer tools</button>
                <button class="filters" @click="filterAdmins">For Admins</button>
                <button class="filters" @click="filterBusiness">For Business</button>
            </div>
            <div>
                <hr style="width: 89%; margin-top: -2px;" />
            </div>
        </header>

        <header class="layout-cards">
            <div class="row row-cols-1 row-cols-md-3 g-4">

                <div v-if="business.valueOf(true)">
                <div class="col">
                    <div class="card">
                    <div class="card-body">
                        <div class="card-body-style">
                            <div class="card-body-image">
                            <img class="card-icon" src="@/assets/business-icon.svg" style="background-color: rgba(41, 156, 219, 0.10);" />
                            <p class="card-text-title">Manage Business</p>
                            </div>
                            <div>
                            <p class="newnote" v-if="count > 0">{{ count }} New</p>
                            <p v-else></p>
                            </div>
                        </div>
                            <div>
                                <p class="card-text-body">Assign application access to businesses at a Super Admin level.</p>
                            </div>
                        </div>
                        <hr style="margin-bottom: 0px;" />
                        <button class="card-button">Launch</button>
                    </div>
                </div>
                </div>

                <div v-if="admins.valueOf(true)">
                <div class="col">
                    <div class="card">
                    <div class="card-body">
                        <div class="card-body-style">
                            <div class="card-body-image">
                            <img class="card-icon" src="@/assets/manage-account-icon.svg" style="background-color: #FFFBEB;" />
                            <p class="card-text-title">Manage User</p>
                            </div>
                            <div>
                            <p class="newnote" v-if="count > 0">{{ count }} New</p>
                            <p v-else></p>
                            </div>
                        </div>
                            <div>
                                <p class="card-text-body">Create and manage your user all from a single dashboard.</p>
                            </div>
                        </div>
                        <hr style="margin-bottom: 0px;" />
                        <button class="card-button">Launch</button>
                    </div>
                </div>
                </div>

                <div v-if="admins.valueOf(true)">
                <div class="col">
                    <div class="card">
                    <div class="card-body">
                        <div class="card-body-style">
                            <div class="card-body-image">
                            <img class="card-icon" src="@/assets/printer-icon.svg" style="background-color: #ECFDF5;" />
                            <p class="card-text-title">Check Printing</p>
                            </div>
                            <div>
                            <p class="newnote" v-if="count > 0">{{ count }} New</p>
                            <p v-else></p>
                            </div>
                        </div>
                            <div>
                                <p class="card-text-body">Streamline employee check management for timely payroll distribution.</p>
                            </div>
                        </div>
                        <hr style="margin-bottom: 0px;" />
                        <button class="card-button">Launch</button>
                    </div>
                </div>
                </div>

                <div v-if="admins.valueOf(true)">
                <div class="col">
                    <div class="card">
                    <div class="card-body">
                        <div class="card-body-style">
                            <div class="card-body-image">
                            <img class="card-icon" src="@/assets/rubric-icon.svg" style="background-color: #FEF2F2;" />
                            <p class="card-text-title">Spread It</p>
                            </div>
                            <div>
                            <p class="newnote" v-if="count > 0">{{ count }} New</p>
                            <p v-else></p>
                            </div>
                        </div>
                            <div>
                                <p class="card-text-body">Streamline your workflow with our easy-to-use spreadsheet tool.</p>
                            </div>
                        </div>
                        <hr style="margin-bottom: 0px;" />
                        <button class="card-button">Launch</button>
                    </div>
                </div>
                </div>

                <div v-if="admins.valueOf(true)">
                <div class="col">
                    <div class="card">
                    <div class="card-body">
                        <div class="card-body-style">
                            <div class="card-body-image">
                            <img class="card-icon" src="@/assets/accounting-icon.svg" style="background-color: #ECFDF5;;" />
                            <p class="card-text-title">Accounting</p>
                            </div>
                            <div>
                            <p class="newnote" v-if="count > 0">{{ count }} New</p>
                            <p v-else></p>
                            </div>
                        </div>
                            <div>
                                <p class="card-text-body">Track and manage paid and received invoices.</p>
                            </div>
                        </div>
                        <hr style="margin-bottom: 0px;" />
                        <button class="card-button">Launch</button>
                    </div>
                </div>
                </div>

                <div v-if="admins.valueOf(true) || business.valueOf(true)">
                <div class="col">
                    <div class="card">
                    <div class="card-body">
                        <div class="card-body-style">
                            <div class="card-body-image">
                            <img class="card-icon" src="@/assets/upload-icon.svg" style="background-color: rgba(75, 56, 179, 0.10);" />
                            <p class="card-text-title">File Uploader</p>
                            </div>
                            <div>
                            <p class="newnote" v-if="count > 0">{{ count }} New</p>
                            <p v-else></p>
                            </div>
                        </div>
                            <div>
                                <p class="card-text-body">Keep track of all funded payroll invoices.</p>
                            </div>
                        </div>
                        <hr style="margin-bottom: 0px;" />
                        <button class="card-button">Launch</button>
                    </div>
                </div>
                </div>

                <div v-if="admins.valueOf(true)">
                <div class="col">
                    <div class="card">
                    <div class="card-body">
                        <div class="card-body-style">
                            <div class="card-body-image">
                            <img class="card-icon" src="@/assets/zendesk.svg" />
                            <p class="card-text-title">Payments Recieved</p>
                            </div>
                            <div>
                            <p class="newnote" v-if="count > 0">{{ count }} New</p>
                            <p v-else></p>
                            </div>
                        </div>
                            <div>
                                <p class="card-text-body">Manage and confirmed all recorded payroll payments from customers.</p>
                            </div>
                        </div>
                        <hr style="margin-bottom: 0px;" />
                        <button class="card-button">Launch</button>
                    </div>
                </div>
                </div>

                <div v-if="admins.valueOf(true)">
                <div class="col">
                    <div class="card">
                    <div class="card-body">
                        <div class="card-body-style">
                            <div class="card-body-image">
                            <img class="card-icon" src="@/assets/jira.svg" />
                            <p class="card-text-title">Groups</p>
                            </div>
                            <div>
                            <p class="newnote" v-if="count > 0">{{ count }} New</p>
                            <p v-else></p>
                            </div>
                        </div>
                            <div>
                                <p class="card-text-body">Create, share and save groups that are referenced frequently within the S3V!N system.</p>
                            </div>
                        </div>
                        <hr style="margin-bottom: 0px;" />
                        <button class="card-button">Launch</button>
                    </div>
                </div>
                </div>

                <div v-if="admins.valueOf(true) || business.valueOf(true)">
                <div class="col">
                    <div class="card">
                    <div class="card-body">
                        <div class="card-body-style">
                            <div class="card-body-image">
                                <img class="card-icon" src="@/assets/dropbox.svg" />
                            <p class="card-text-title">Reports</p>
                            </div>
                            <div>
                            <p class="newnote" v-if="count > 0">{{ count }} New</p>
                            <p v-else></p>
                            </div>
                        </div>
                            <div>
                                <p class="card-text-body">Generate and download reports custom reports.</p>
                            </div>
                        </div>
                        <hr style="margin-bottom: 0px;" />
                        <button class="card-button">Launch</button>
                    </div>
                </div>
                </div>
            </div>
        </header>
        <header class="pagenav">
            <div>
                <hr style="margin-bottom: -10px;"/>
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
body {
    min-width: 100vw;
}

.upper {
    background-color: #0C111D;
    width: 100%;
}

.lower {
    color: black;
    margin-top: 32px;
    width: 100%;
}

.middle {
    margin-top: 10px;
    margin-left: 5.5%;
    width: 100%;
}

.layout-cards {
    margin-left: 5.5%;
    width: 89%;
    margin-top: 24px;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-evenly;
}

.pagenav {
    margin-left: 5.5%;
    margin-right: 5.5%;
}

nav {
    align-items: center;
    display: flex;
    flex-direction: row;
    width: 100%;
    justify-content: space-between;
}

.pagecont {
    padding-top: 0px;
    display: flex;
    flex-direction: row;
    align-items: center;
}

.logo {
    margin-right: 10px;
    height: 39.75px;
    width: 45px;
    background: transparent;
}

.generalicon {
    height: 40px;
    padding: 8px;
    border-radius: 10px;

    &:hover {
        background-color: #182230;
        cursor: pointer;
    }
}

.profile {
    width: 40px;
    height: 40px;
    border-radius: 50px;

    &:hover {
        background-color: #182230;
        cursor: pointer;
    }
}

.home {
    color: #FFF;
    font-size: 16px;
    background-color: transparent;
    border-style: none;
    padding: 8px 12px;
    border-radius: 6px;

    &:hover {
        background-color: #182230;
        cursor: pointer;
    }
}

.toptext {
    color: #FFF;
    display: flex;
    flex-direction: row;
    align-items: center;
}

.lowertext {
    color: #030712;
}

.apppermission {
    color: #475467;
    font-weight: 600;
    background-color: white;
    font-size: 14px;
    border-radius: 5px;
    padding: 10px 14px;
    border: 1px solid #E5E7EB;

    &:hover {
        cursor: pointer;
    }
}

.filters {
    color: #667085;
    font-weight: 600;
    font-size: 14px;
    padding-bottom: 12px;
    border-style: none;
    background-color: transparent;

    &:hover {
        color: #059669;
        border-bottom: 2px solid #10B981;
        cursor: pointer;
    }
}

.pagenavfont {
    margin-top: 12px;
    align-items: center;
    display: flex;
    flex-direction: row;
    font-size: 14px;
    font-weight: 600;
    color: #475467;

    &:hover {
        cursor: pointer;
    }
}

.card-button {
    width: 180%;
    align-content: end;
    font-weight: bold;
    font-size: 14px;
    border: none;
    background-color: transparent;
    padding: 8px 0px;

    &:hover {
        cursor: pointer;
    }
}

.newnote {
    color: #DC2626;
    margin-bottom: 15px;
    padding: 1px 7px;
    background-color: #FEF2F2;
    border-radius: 20px;
    font-weight: 600;
}

.card-icon {
    border-radius: 5px;
    padding: 5px;
    width: 40px;
}

.card-body{
    margin-top: -10px;
}

.card-body-style{
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
}

.card-body-image{
    display: flex;
    flex-direction: row;
    align-items: center;
}
.card-text-title{
    padding-left: 10px; 
    font-size: 16px;
    font-weight: bold;
    margin-top: 10px;
}

.card-text-body{
    margin-top: 5px;
    margin-bottom: -15px;
}
</style>
