<script>
export default{
    name: 'AppFooter',
    data() {
    return {
        posts: [
            {
                "first-posts" : '<i class="fa-brands fa-facebook-f"></i> ',
                "second-posts" : '<i class="fa-brands fa-twitter"></i>',
                "third-posts" :'<i class="fa-brands fa-youtube"></i>',
                
                
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
    <div class="ms-container-large">
        <div class="d-flex">
            <ul>
                <li v-for="cours in courses">{{ cours.arts }}</li>
                <li v-for="cours in courses">{{ cours.business }}</li>
            </ul>
        </div>

    </div>

</template>

<style scoped lang="scss">
.ms-container-large{
    width: 95%;
    margin: 0 auto;
}
</style>