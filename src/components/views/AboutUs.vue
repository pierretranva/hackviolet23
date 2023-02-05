<template>
    <div>
        <div id="header">
            <h1>
                About Us
            </h1>
        </div>
        <img src="../../assets/torgBridge.png"/>
        <div>
        
            <h5>We are a group of undergraduate Computer Science students at Virginia Tech. Our mission aims to cultivate and foster welcoming
            experiences for underrepresented groups in the College of Engineering by providing helpful resources through our website. Thank you
            for visiting!</h5>
            <p>
            <b id="bold">Hannah Nguyen:</b> I'm a freshman General Engineering major interested in HCI, technology ethics, and the relationship between race and 
            technology as master categories. My hobbies include digital art, fashion, and music! I'm a current graphics organizer for VT Hacks 
            and an active member of both SASE, VSA, and FASA.
            <br><br>
            <b id="bold"> Vy Dinh:</b> I'm a sophomore majoring in Computer Science with a minor in Mathematics. I'm a part of KASA, SASE, VSA, SWE, and Hokie Ambassadors.
            I hope our project can help future freshmen in engineering adjust to Virginia Tech and grant them the resources to succeed and network!
            <br><br>
            <b id="bold">Pierre Tran:</b> I'm currently a freshman majoring in Computer Science with a minor in Mathematics. I'm a member of SASE, VSA, and FASA. I like to go to the gym, sleep and eat.
            <br><br>
            <b id="bold">Jinju Brown:</b> I'm a freshman currently studying General Engineering, but planning to major in Computer Science. I'm a member of CAS, SASE, KASA, 
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
#bold{
    font-weight: bold;
}
p {
    margin: 0;
    padding: 0;
}
img {
    width: 100%;
    margin-top:-10rem;
    margin-bottom: -15rem;
}
</style>
