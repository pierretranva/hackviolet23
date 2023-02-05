<template>
    <div>
        <div id="header">
            <h1>
                About Us
            </h1>
        </div>
        <img id="torg" src="../../assets/torgBridge.png"/>
        
        <div>
        
            <h5>We are a group of undergraduate Computer Science students at Virginia Tech. Our mission aims to cultivate and foster welcoming
            experiences for underrepresented groups in the College of Engineering by providing helpful resources through our website. Thank you
            for visiting!</h5> 
            <div class="badge-grid">
                <a href="#first"> 
                    <img class="badge" alt="Hannah Nguyen" src="https://img.shields.io/badge/-Hannah%20Nguyen-brightgreen" />
                </a>
                <a href="#second">
                    <img class="badge" alt="Vy Dinh" src="https://img.shields.io/badge/-Vy%20Dinh-%23A16B16" />
                </a>
                <a href="#third">
                    <img class="badge" alt="Pierre Tran" src="https://img.shields.io/badge/-Pierre%20Tran-%2373BDA8" />
                </a>
                <a href="#fourth">
                    <img class="badge" alt="Jinju Brown" src="https://img.shields.io/badge/-Jinju%20Brown-%23D2AD2C" />
                </a>
                
            </div>
            <p>
            <b id="first">Hannah Nguyen:</b> I'm a freshman General Engineering major interested in HCI, technology ethics, and the relationship between race and 
            technology as master categories. My hobbies include digital art, fashion, and music! I'm currently a graphics organizer for VT Hacks 
            and an active member of SASE, VSA, and FASA.
            <br><br>
            <b id="second"> Vy Dinh:</b> I'm a sophomore majoring in Computer Science with a minor in Mathematics. I'm a part of KASA, SASE, VSA, SWE, and Hokie Ambassadors.
            I hope our project can help future freshmen in engineering adjust to Virginia Tech and grant them the resources to succeed and network!
            <br><br>
            <b id="third">Pierre Tran:</b> I'm currently a freshman majoring in Computer Science with a minor in Mathematics. I'm a member of SASE, VSA, and FASA. I like to go to the gym, sleep, and eat.
            <br><br>
            <b id="fourth">Jinju Brown:</b> I'm a freshman currently studying General Engineering, but planning to major in Computer Science. I'm a member of CAS, SASE, KASA, 
            and the Galipatia Community. Throughout my years of wanting to become an engineer, I wished that I had a resource like this to help me through
            my process.
        </p>
        </div>
    </div>
</template>

<style scoped>
/*-------------------------------------------*\
    CSS Normalisation 
\*-------------------------------------------*/
#header{
    display: flex;
    justify-content: center;
}
#first, #second, #third, #fourth{
    font-weight: bold;
}
p {
    margin: 0;
    padding: 0;
}
#torg {
    width: 100%;
    margin-top:-10rem;
    margin-bottom: -15rem;
}
.badge-grid {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: center;
    margin-top: 20px;
    margin-bottom: 3vh;
    justify-content: space-between;
    width: 80%;
    transform: translateX(10%);
}
.badge {
    width: auto;
    height: 20px;
    border-radius: 0px;
    font-size: 12px;
    margin-right:100%;
}
</style>
