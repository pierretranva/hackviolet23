<template>
    <div>

        <div id="header">
            <h1>
                Resources
            </h1>
        </div>
        <h5>Creating your own schedule can be stressful and intimidating, especially when you're a first year. Here are
            some useful tips and resources to help you get started and build the perfect schedule fit for you. </h5>
        
        <div class="badge-grid">
            <a href="#1"> 
                <img class="badge" alt="Rate My Professor" src="https://img.shields.io/badge/-Rate%20My%20Professor-brightgreen" />
            </a>
            <a href="#2">
                <img class="badge" alt="PScheduler" src="https://img.shields.io/badge/-PScheduler-%23A16B16" />
            </a>
            <a href="#3">
                <img class="badge" alt="Anaau" src="https://img.shields.io/badge/-Anaau-%23CC6B49" />
            </a>
            <a href="#4">
                <img class="badge" alt="Coursicle" src="https://img.shields.io/badge/-Coursicle-%23D2AD2C" />
            </a>
            <a href="#5">
                <img class="badge" alt="Course Pickle" src="https://img.shields.io/badge/-Course%20Pickle-%2373BDA8" />
            </a>
        </div>

       
        <div id="list">
        <ol>
            <li id="1"><p>After deciding your classes, it's important to research the professors. <a href="https://www.ratemyprofessors.com/">Rate My Professor</a> 
                is a popular website used to check
                different factors about your professors including workload, classroom environment, teaching style,
                homework/test policies, and more. Often times, students walk into their first day of class blind without
                knowing this crucial information, and on the off chance you don't get along with you're professor, it's
                difficult to switch into another section before the add/drop period closes.</p></li>
            <img src="../../assets/ratemyprofessor.jpg" />
            <li id="2">
            With so many classes, it's difficult to plan the times for all your classes. Some might prefer early
            classes while others afternoon classes. Some might want their classes evenly spaced throughout the week
            while others might want them crowded in the beginning to leave Friday free. All these options may be
            overwhelming, but <a href="https://pscheduler.com/">PScheduler</a> is a useful website that can help relieve
            this stress. After inputing your classes for the semester, PScheduler is able to generate all the different
            combinations of schedules you could have. You can shuffle through each schedule until you find a one that
            works for you.
            </li>
           
            <img src="../../assets/pscheduler.jpg" />
            <li id="3"><p>
            Another great website is <a href="https://anaanu.com/?universities">Anaanu</a> which can be used to check
            grade records for all your classes. It will list the average GPA in the course along with the grade
            distribution. In addition, it will list the grade distribution for all the professors teaching the course.
            Anaanu is great for figuring out your courseload for the semester. This way, you can create a schedule that
            has a balance between easy and difficult classes.</p>
            </li>
            <li id="4"><p>
            Navigating Hokie Spa to find your schedule can be inconvienent and annoying. <a
                href="https://www.coursicle.com/">Coursicle</a> is an app that puts all your classes into a timetable
            and stores information for each class such as the professor, location, time, and course description. It's an
            easy and accessible way to keep your schedule on your phone, and the blocking layout makes it simply to
            read.</p>
        </li>
            <li id="5"><p>
            If you're in need of switching to another class or section that's full, <a
                href="https://coursepickle.com/">Course Pickle</a> is a website that can send you emails or text
            messages to alert you of an opening in the course. There is a small fee for text messages, but email alerts
            are completely free and you can sign up for as many classes as you want.</p>
            </li>
        </ol>
        </div>
    </div>
</template>

<style scoped>
/*-------------------------------------------*\
    CSS Normalisation 
\*-------------------------------------------*/
#header {
    display: flex;
    justify-content: center;
}

p {
    margin: 0;
    padding: 0;
}

img {
    display: block;
    margin-left: auto;
    margin-right: auto;
    width: 30%;
}
li{
    list-style: decimal;
    font-weight: 100;
    margin-bottom: 3vh ;
}
.badge-grid {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    align-items: center;
    margin-top: 20px;
    justify-content: space-around;
    width: 80%;
    transform: translateX(10%);
}
.badge {
    width: auto;
    height: 20px;
    border-radius: 0px;
    font-size: 12px;
    padding-right: 0px;
}
ol > img{
    margin-bottom: 3vh;
}
</style>
