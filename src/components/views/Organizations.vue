<template>
    <div class="outside">
        <h1>
            Organizations
        </h1>
        <h5>Virginia Tech offers many organizations that can help women form valuable connections and provide support
            from other strong women. These organizations also provide many opportunities for professional development.
        </h5>
        <div class="badge-grid">
            <a href="#1"> 
                <img class="badge" alt="SASE" src="https://img.shields.io/badge/-SASE-brightgreen" />
            </a>
            <a href="#2">
                <img class="badge" alt="AWC" src="https://img.shields.io/badge/-AWC-%23A16B16" />
            </a>
            <a href="#3">
                <img class="badge" alt="Hypatia" src="https://img.shields.io/badge/-Hypatia-%23CC6B49" />
            </a>
            <a href="#4">
                <img class="badge" alt="SWE" src="https://img.shields.io/badge/-Society%20of%20Women%20Engineers-%2373BDA8" />
            </a>
        </div>
        <h2 id="1">
            SASE
        </h2>
        <img id="sase" src="../../assets/sase.png" />
        <p>
            The Society of Asian Scientists and Engineers celebrates diversity in STEM and provides career opportunities
            as well
            as professional development workshops. Join to connect with mentors, alumni, and form relationships with
            like minded individuals.
            <br><br>
            "SASE helped me meet with a mentor from a similar cultural background who I formed a personal relationship
            with
            and gave me the resources to build an appealing resume." -Pierre Tran
            <br><br>
        </p>
        <h2 id="2">
            AWC
        </h2>
        <img id="awc" src="../../assets/awc.png" />
        <p>
            The Association For Women in Computing is a nonprofit, student run organization that promotes gender equality
            in computing.
            Their work includes providing support for women in technological fields and organizing HackViolet,
            their flagship hackathon.
            <br><br>
        </p>
        <h2 id="3">
            Hypatia
        </h2>
        <img src="../../assets/hypatia.png" />
        <p>
            Hypatia is a living learning community for freshman and first-time women engineers. Members of Hypatia are
            put in mentor groups
            for help with professional development and support in the transition into engineering at Virginia Tech.
            <br><br>
            "The professional development workshops helped me to become a well-rounded engineer." -Jinju Brown
            <br><br>
        </p>
        <h2 id="4">
            SWE
        </h2>
        <img id="swe" src="../../assets/swe.png" />
        <p>
            The Society of Women Engineers contributes to gender inclusivity at Virginia Tech by providing weekly
            outreach, social, and
            professional development activities. SWE participates in the annual SWE conference which hosts the world's
            largest career fair
            for women in engineering and technology.
            <br><br>
            "SWE is a great way to connect with female engineers because you don't see them very often within your
            classes. The female
            speakers and convention help me combat my imposter syndrome." -Vy Dinh
            <br><br>
        </p>
    </div>
</template>

<style scoped>
/*-------------------------------------------*\
    CSS Normalisation 
\*-------------------------------------------*/
p {
    margin: 0;
    padding: 0;

}

div {
    display: flex;
    justify-content: center;
    flex-direction: column;
}

img {
    width: 80%;
    max-width: 300px;
    display: block;
    margin-left: auto;
    margin-right: auto;

}

h2 {
    display: block;
    margin-left: auto;
    margin-right: auto;

}

h1 {
    display: block;
    margin-left: auto;
    margin-right: auto;

}

#sase {
    margin-top: -6vh;
    margin-bottom: -3vh;
}

#awc {
    margin-top: 2vh;
    margin-bottom: 5vh;
}

#swe {
    margin-top: -4vh;
}
.badge-grid {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: center;
    margin-top: 20px;
    justify-content: space-between;
    width: 100%;
}
.badge {
    width: auto;
    height: 20px;
    border-radius: 0px;
    font-size: 12px;
    padding-right: 0px;
}
</style>