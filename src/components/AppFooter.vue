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
                        <li class="mb-1 d-flex"> <i class="fa-solid fa-house mt-1 me-2"></i> Residential Location <br> 9521 Broadsberry Avenue <br> Paddington RC7 9ZA</li> 
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

                    
                    
                    

            <ul >
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
                <a href=""><li v-for="cours in courses">{{ cours.arts }}</li> </a>
                <a href=""><li v-for="cours in courses">{{ cours.business }}</li></a>
                <a href=""><li v-for="cours in courses">{{ cours.engineering}}</li></a>
                <a href=""><li v-for="cours in courses">{{ cours.medicine }}</li></a>
                <a href=""><li v-for="cours in courses">{{ cours.sciences }}</li></a>
                <div class="mt-5">
                    <h6>ADMISSIONS</h6>
                    <a href=""><li v-for="text in admissions">{{ text.text }}</li></a>
                </div>
            </ul>

                
                

            <ul>
                <h6>RESOURCES</h6>
                <a href=""><li v-for="resource in resources">{{ resource.campus }}</li></a>
                <a href=""><li v-for="resource in resources">{{ resource.calendar }}</li></a>
                <a href=""><li v-for="resource in resources">{{ resource.club }}</li></a>
                <a href=""><li v-for="resource in resources">{{ resource.program }}</li></a>
                <a href=""><li v-for="resource in resources">{{ resource.staff }}</li></a>
                <div class="mt-5">
                    <h6>QUICLINKS</h6>
                    <a href=""><li v-for="text in quicklinks">{{ text.text }}</li></a>
                 </div>
             </ul>
             
             
             
             <ul>
                 <h6> UPCOMING EVENTS</h6>
                 <div>
                     <a href=""><li v-for="event in eventsBusinees"> {{ event.title }}</li></a>
                     <a href=""><li v-for="event in eventsBusinees"> {{ event.date }}</li></a>
                     <a href=""><li v-for="event in eventsBusinees"> {{ event.place }}</li></a>
                 </div>
                 <div class="mt-3">
                     <a href=""><li v-for="event in eventsPolitics"> {{ event.title }}</li></a>
                     <a href=""><li v-for="event in eventsPolitics"> {{ event.date }}</li></a>
                     <a href=""><li v-for="event in eventsPolitics"> {{ event.place }}</li></a>
                 </div>
            </ul>
            
        </div>

        <div class="d-flex justify-content-between color-gray">
            <div class="left">
                <ul class="d-flex gap-1">
                    <li>ok</li>
                    <li>ok</li>
                    <li>ok</li>
                    <li>ok</li>
                    <li>ok</li>
                </ul>
            </div>

            <div class="right">
                    <nav>
                       <ul class="d-flex list-unstyled gap-3 ">
                         <a href=""> <li v-html="socialInfo.fb"></li></a>
                         <a href=""><li v-html="socialInfo.twitter"></li></a>
                         <a href=""><li v-html="socialInfo.yt"></li></a>
                         <a href=""><li v-html="socialInfo.insta"></li></a>
                        </ul>
                    </nav>
             </div>
                
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
</style>