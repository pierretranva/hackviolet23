<template>
    <div>
        <div id="title">
            <h2>
                Notable Alumni
            </h2>
        </div>
        <div id="body">
            <h5>There are many examples of successful women who are Virginia Tech Alumni. These women below show us that
                it is always possible to overcome the odds and become successful as a woman in STEM! </h5>
            <img src="../../assets/AmyElliot.jpg" />
            <h4>
                Amy Elliot '14
            </h4>
            <p>
                She created a 3D-printed statue that was displayed at the Smithsonian for their Women's History Month
                exhibit
            </p>
            <div class="divider"></div>
            <img src="../../assets/CarlaRampy.jpg" />
            <h4>Carla Rampy '99</h4>
            <p>
                Currently the President and CEO of Quality Agents
            </p>
            <div class="divider"></div>
            <img src="../../assets/lisafinneran.jpg" />
            <h4>Lisa Finneran '85</h4>
            <p>
                Leads a engineer group and runs GDMS engineering
            </p>
            <div class="divider"></div>
            <img src="../../assets/SarahFranklin.jpg" />
            <h4>Sarah Frankin '97</h4>
            <p>
                President and chief marketing officer of Salesforce
            </p>
            <div class="divider"></div>
            <img src="../../assets/stacybranham.jpg" />
            <h4>Stacey Branham '07 '14</h4>
            <p>
                Awarded the 2022 Virginia Tech Department of Computer Science Distinguished Early Career Alumni Awarded
            </p>
        </div>
    </div>
</template>

<style scoped>
/*-------------------------------------------*\
    CSS Normalisation 
\*-------------------------------------------*/

p {
    margin-bottom: 5vh;
    padding: 0;
}

img {
    width: 80%;
}

#title {
    display: flex;
    justify-content: center;
}

#body {
    display: flex;
    flex-direction: column;
}

#body>img {
    align-self: center;
}

#body>h4 {
    align-self: center;
    margin-bottom: 0;
}
</style>
