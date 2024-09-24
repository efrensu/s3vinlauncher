<script>

</script>

<template>
    <header>
        <!--Section:Filters-->
        <ul>
            <li>View all</li>
            <li>Developer tools</li>
            <li>For Admins</li>
            <li>For Businesses</li>
        </ul> 

        <!--Section:First Row-->
        <div class="layout-top">
            <div class="outerborder">
                <div class="inner">
                    <div class="maintitle">
                        <img class="business" src="@/assets/business-icon.svg"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Manage Business</p>
                    </div>
                    <p>Assign application access to businesses at a Super Admin level.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button>Launch</button>
            </div>
            <div class="outerborder" style="margin-left: 20%;">
                <div class="inner">
                    <div class="maintitle">
                        <img class="accounts" src="@/assets/manage-account-icon.svg"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Manage User</p>
                    </div>
                    <p>Create and manage your user all from a single dashboard.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button>Launch</button>
            </div>
            <div class="outerborder" style="margin-left: 40%;">
                <div class="inner">
                    <div class="maintitle">
                        <img class="checks" src="@/assets/printer-icon.svg"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Check Printing</p>
                    </div>
                    <p>Streamline employee check management for timely payroll distribution</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button>Launch</button>
            </div>
        </div>

        <!--Section:Second Row-->
        <div class="layout-middle">
            <div class="outerborder">
                <div class="inner">
                    <div class="maintitle">
                        <img class="rubric" src="@/assets/rubric-icon.svg"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Spread It</p>
                    </div>
                    <p>Streamline your workflow with our easy-to-use spreadsheet tool.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button>Launch</button>
            </div>
            <div class="outerborder" style="margin-left: 20%;">
                <div class="inner">
                    <div class="maintitle">
                        <img class="generalicon" src="@/assets/accounting-icon.svg" style="background-color: #ECFDF5;;"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Accounting</p>
                    </div>
                    <p>Track and manage paid and received invoices.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button>Launch</button>
            </div>
            <div class="outerborder" style="margin-left: 40%;">
                <div class="inner">
                    <div class="maintitle">
                        <img class="generalicon" src="@/assets/upload-icon.svg" style="background-color: rgba(75, 56, 179, 0.10);"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">File Uploader</p>
                    </div>
                    <p>Keep track of all funded payroll invoices.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button>Launch</button>
            </div>
        </div>

        <!--Section:Third Row-->
        <div class="layout-lower">
            <div class="outerborder">
                <div class="inner">
                    <div class="maintitle">
                        <img class="generalicon" src="@/assets/zendesk.svg"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Payments Recieved</p>
                    </div>
                    <p>Assign application access to businesses at a Super Admin level.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button>Launch</button>
            </div>
            <div class="outerborder" style="margin-left: 20%;">
                <div class="inner">
                    <div class="maintitle">
                        <img class="generalicon" src="@/assets/jira.svg"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Groups</p>
                    </div>
                    <p>Create, share and save groups that are referenced frequently within the S3V!N system.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button>Launch</button>
            </div>
            <div class="outerborder" style="margin-left: 40%;">
                <div class="inner">
                    <div class="maintitle">
                        <img class="generalicon" src="@/assets/dropbox.svg"/>
                        <p style="padding-left: 10px; font-size: 16px;font-weight: bold;">Reports</p>
                    </div>
                    <p>Generate and download reports custom reports.</p>
                </div>
                <hr style="border: 1px solid #E5E7EB;" />
                <button>Launch</button>
            </div>
        </div>

    </header>
</template>

<style scoped>

header{
    margin-top: 10%;
    width: 100%;
    position: fixed;
}

.layout-top{
    margin-left: 7.8%;
    display: flex;
    flex-direction: row;
    align-content: center;
    width:100%;
    margin-top: 1%;

}

.layout-middle{
    margin-left: 7.8%;
    display: flex;
    flex-direction: row;
    align-content: center;
    width:100%;
    margin-top: 7%;

}

.layout-lower{
    margin-left: 7.8%;
    display: flex;
    flex-direction: row;
    align-content: center;
    width:100%;
    margin-top: 7%;

}

.outerborder{
    width: 18%;
    font-weight: bold;
    background-color: white;
    font-size: 14px;
    border-radius: 10px;
    margin-top: 10px;
    border: 2px solid #E5E7EB;
    position: fixed;
}

.inner{
    margin-left: 15px;
    margin-top: 10px;
    margin-bottom: 15px;
    color: black;
}

.maintitle{
    display: flex;
    flex-direction: row;
    padding: 20px 0px;
    width:90%;
    margin: 0;
}

button{
    margin-top: 10px;
    margin-bottom: 10px;
    font-weight: bold;
    font-size: 14px;
    border: none;
    background-color: transparent;
    margin-left: 80%;
}

ul{
    margin-left: 6.3%;
    font-weight: 600;
    margin-top: 35px;
    display: flex;
    flex-direction: row;
    align-items: center;
    list-style:none;
}

li{
    font-size: 14px;
    padding-right: 20px;
    color: #667085;
    border-bottom:2px solid #E5E7EB;
    padding-bottom: 11px;

    &:hover{
        color: #059669;
        padding-bottom: 11px;
        border-bottom: #10B981;
        border-bottom: solid 2px;
    }
}

.business{
    padding: 5px;
    width: 30px;
    background-color: rgba(41, 156, 219, 0.10);
}

.accounts{
    padding: 5px;
    width: 30px;
    background-color: #FFFBEB;
}

.checks{
    padding: 5px;
    width: 30px;
    background-color: #ECFDF5;
}

.rubric{
    padding: 5px;
    width: 30px;
    background-color: #FEF2F2;
}

.generalicon{
    padding: 5px;
    width: 30px;
}

</style>