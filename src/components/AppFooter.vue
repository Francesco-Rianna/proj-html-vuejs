<script>
    export default{
        name: 'AppFooter',
        props : {
            socialInfo : Object , 
           
        },
        data() {
        return {
            posts: [
                
                    {
                        "text":'What do succesful grads think  you should study?',
                        "date" :'March 16 2016'
                    },
                    
                    {
                        "text":'Former student discusses succes in the fashion industry',
                        "date" :'March 15 2016'
                    },
                    {
                        "text":'How do you best prepare for university',
                        "date" :'March 15 2016'
                    },
                ],
             courses: [
                {
                    'arts': 'Arts & Umanities',
                    'business': 'Business & Management',
                    'engineering':'Enginering & Technlology',
                    'medicine' :'Life Sciences & Medicine',
                    'sciences' : 'Natural Sciences'
    
                }
             ],
             resources: [
                {
                    'campus':'Campus Directory',
                    'calendar': 'Academic Calendar',
                    'club' : 'Sport Clubs',
                    'program' : 'Graduate Programs',
                    'staff' : 'Faculty & Staff'
                }
             ],
    
             eventsBusinees :[
                {
                    'title':'Businees Seminar',
                    'date': 'July 1,2019 @8:00 am - July 1, 2021 @ 5:00 pm',
                    'place': 'United States'
                }
             ],
             eventsPolitics :[
                {
                    'title':'Politics Seminar',
                    'date': 'November 6,2021 @8:00 am - November 6, 2021 @ 5:00 pm',
                    'place': 'United Kingdom'
                }
             ],
    
             admissions : [
                {'text': 'Eligibility'},
                {'text': 'Application'},
                {'text': 'Rewiew Process'},
                {'text': 'How to Apply'}
             ],
             quicklinks: [
                {'text': 'University Library'},
                {'text': 'Campus Services'},
                {'text': 'Careers'}
             ],
    
             autors : [
                 {
                    'copy': 'Theme Fusion',
                    'text' : 'All Right Reserved',
                    'powered': 'Powered By WordPress',
                    'mail' : 'support@theme-fusion.com',
                    'number': '1.800.546.456'
                },
             ]
                    
                    
                    
                    
                
                
    
    
            
    
            
            }         
        }
    }
</script>

<template>
    <div class="ms-container-large py-5">
        <div class="d-flex justify-content-around">

            <ul>
                <h6>AVADA UNIVERSIY</h6>
                <div class="color-gray">
                    <a href="">
                        <li class="mb-1 d-flex"> <i class="fa-solid fa-house mt-1 me-2"></i> Residential Location
                            <br> 9521 Broadsberry Avenue
                            <br> Paddington RC7 9ZA</li>
                    </a>
                    <a href="">
                        <li class="mb-1 d-flex"><i class="fa-solid fa-phone-flip mt-1 me-2"></i> 1.800.458.556</li>
                    </a>
                    <a href="">
                        <li class="color-gray-d"> <i class="fa-regular fa-envelope mt-1 me-2"></i> <strong>info@your-domain.com </strong> </li>
                    </a>
                    <a href="">
                        <li class="mt-1"> <i class="fa-regular fa-clock mt-1 me-2"></i> Monday-Friday 8:00 AM 10:00 PM</li>
                    </a>
                </div>
            </ul>





            <ul>
                <h6>RECENT POSTS</h6>
                <a href="">
                    <li v-for="post in posts" class="custom-list mb-3 ms-3">
                        <div class="lh-lg color-gray-d">
                            {{ post.text }}
                        </div>
                        <div class="color-gray">
                            {{ post.date }}
                        </div>

                        <div class="mini-bar"></div>
                    </li>
                </a>
            </ul>


            <ul>
                <h6>COURSES</h6>
                <a href="">
                    <li v-for="cours in courses">{{ cours.arts }}</li>
                </a>
                <a href="">
                    <li v-for="cours in courses">{{ cours.business }}</li>
                </a>
                <a href="">
                    <li v-for="cours in courses">{{ cours.engineering}}</li>
                </a>
                <a href="">
                    <li v-for="cours in courses">{{ cours.medicine }}</li>
                </a>
                <a href="">
                    <li v-for="cours in courses">{{ cours.sciences }}</li>
                </a>
                <div class="mt-5">
                    <h6>ADMISSIONS</h6>
                    <a href="">
                        <li v-for="text in admissions">{{ text.text }}</li>
                    </a>
                </div>
            </ul>




            <ul>
                <h6>RESOURCES</h6>
                <a href="">
                    <li v-for="resource in resources">{{ resource.campus }}</li>
                </a>
                <a href="">
                    <li v-for="resource in resources">{{ resource.calendar }}</li>
                </a>
                <a href="">
                    <li v-for="resource in resources">{{ resource.club }}</li>
                </a>
                <a href="">
                    <li v-for="resource in resources">{{ resource.program }}</li>
                </a>
                <a href="">
                    <li v-for="resource in resources">{{ resource.staff }}</li>
                </a>
                <div class="mt-5">
                    <h6>QUICLINKS</h6>
                    <a href="">
                        <li v-for="text in quicklinks">{{ text.text }}</li>
                    </a>
                </div>
            </ul>



            <ul>
                <h6> UPCOMING EVENTS</h6>
                <div class="d-flex">
                    <div class="calendar me-2">
                        <div class=" d-flex justify-content-center">
                            <div class="square mt-1 d-flex justify-content-center align-items-center color-orange"> Fri</div>
                        </div>
                        <div class="d-flex justify-content-center color-white">27</div>
                    </div>
                    <div class="mb-3">
                        <a href="">
                            <li v-for="event in eventsBusinees"> {{ event.title }}</li>
                        </a>
                        <a href="">
                            <li v-for="event in eventsBusinees"> {{ event.date }}</li>
                        </a>
                        <a href="">
                            <li v-for="event in eventsBusinees"> {{ event.place }}</li>
                        </a>
                    </div>
                </div>

                <div class="d-flex mt-4 align-items-center">
                    <div class="calendar me-2 ">
                        <div class=" d-flex justify-content-center">
                            <div class="square mt-1 d-flex justify-content-center align-items-center color-orange"> Fri</div>
                        </div>
                        <div class="d-flex justify-content-center color-white">27</div>
                    </div>

                    <div class="">
                        <a href="">
                            <li v-for="event in eventsPolitics"> {{ event.title }}</li>
                        </a>
                        <a href="">
                            <li v-for="event in eventsPolitics"> {{ event.date }}</li>
                        </a>
                        <a href="">
                            <li v-for="event in eventsPolitics"> {{ event.place }}</li>
                        </a>
                    </div>
                </div>
                <div class="mt-4"> <a href="">View more... </a> </div>

            </ul>


        </div>


    </div>

    <div class="d-flex justify-content-between color-gray mt-3 py-1 ms-container-large">
        <div class="left">
            <ul class="d-flex gap-1">
                <li class="d-flex align-items-center" v-for="autor in autors"> <i class="fa-regular fa-copyright mt-1 me-1"></i> {{ autor.copy }} <span class="ms-2"> | </span> </li>
                <li v-for="autor in autors"> {{ autor.text }} <span class="ms-2"> | </span></li>
                <li v-for="autor in autors"> {{ autor.powered }} <span class="ms-2"> | </span></li>
                <li v-for="autor in autors"> {{ autor.mail }} <span class="ms-2"> | </span></li>
                <li v-for="autor in autors"> {{ autor.number }} <span class="ms-2"> | </span></li>
            </ul>
        </div>

        <div class="right">
            <nav>
                <ul class="d-flex list-unstyled gap-3 ">
                    <a href="">
                        <li v-html="socialInfo.fb"></li>
                    </a>
                    <a href="">
                        <li v-html="socialInfo.twitter"></li>
                    </a>
                    <a href="">
                        <li v-html="socialInfo.yt"></li>
                    </a>
                    <a href="">
                        <li v-html="socialInfo.insta"></li>
                    </a>
                </ul>
            </nav>
        </div>

    </div>






</template>

<style scoped lang="scss">
    @use '../style/variables' as *;
    .ms-container-large{
        width: 95%;
        margin: 0 auto;
    }
    
    li {
        list-style: none;
        font-size: 13px;
    }
    
    .custom-list {
        list-style: '>  ';
    }
    
    .mini-bar {
        width: 280px; 
        height: 1.5px; 
        background-color:#f7f5f4;
        
        margin-top: 10px; 
    }
    
    .color-gray{
        color : $color-gray
    }
    
    .color-gray-d{
        color: $color-gray-d
    }
    
    .color-white{
        color: $color-white;
    }
    
    .color-orange{
       color: $color-orange
    }
    
    .left{
        i{
            font-size: 10px;
        }
    }
    
    .calendar {
        width: 40px;
        height: 60px;
        background-color: $color-orange;
    }
    
    .square {
        width: 90%;
        height: 30px;
        background-color: $color-white;
    }
</style>