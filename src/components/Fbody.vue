<template>
    <div>
        <b-card-group deck>
            <b-card
                border-variant="primary"
                header="அவளை பற்றி கவிதை வரிகளில் இருந்து துவங்குகிறேன்"
                header-bg-variant="primary"
                header-text-variant="white"
                align="center"
            >
                <b-card-text>இந்த இடத்தில் நான் கடல் அலையாகவும், நீ பௌர்ணமி நிலவாகவும் உன்னை கற்பனையாக நினைத்து கொள்கிறேன்.</b-card-text><br />
                <b-card-text>ஏனனில், நிலவின் ஒளி கடல் அலைகளின் மீது படும் போது தான் அதன் அழகு அதிகமா தெரியும்..</b-card-text>
                <b-card-text>அது போல தான் நீ ஏன் அருகினில் இருக்கும் போது மட்டும் தான் என் வாழ்க்கை அழகாகவும் அர்த்தமுள்ளதாகவும் இருக்கும் என்பதை தெரிவித்து கொள்கிறேன் 😊</b-card-text>
            </b-card>
        </b-card-group>
        <b-container>
            <b-row class="text-center mt-3" align-v="center">
                <b-col><b-button class="main-navigation-button" @click="show_hide_div = true" variant="primary">இப்போது அவளை பற்றி பாப்போம்</b-button></b-col>
            </b-row>
        </b-container>

        <div v-if="show_hide_div">
            <b-card-group deck class="mt-3">
            <b-card
                border-variant="primary"
                header="அவள் ஒரு வாயாடி"
                header-bg-variant="primary"
                header-text-variant="white"
                align="center"
            >
                <b-card-text>இந்த இடத்தில அவள் ஒரு வாயாடி என்பதை சொல்லியே ஆக வேண்டும். like bajari 😁</b-card-text><br />
                <b-card-text>பேச ஆரம்பித்தால் பேசி கொண்டே இருப்பாள். அவள் எப்படி பேசுவாள் என்றால் நாம் உம் உம் சொல்லியே நமக்கு தொண்டை வலி வந்து விடும். அந்த அளவிற்கு பேசுவாள் 😅😂</b-card-text>
                <b-card-text>இருந்தாலும் அது எனக்கு சலிப்பவே இருக்காது. அதையும் நான் அவளுக்கு தெரியாமல் ரசிப்பேன்</b-card-text>
                <b-card-text>இதை சொல்ல மறந்துட்டனே. பொறுமையவே பேச மாட்டா எக்ஸ்பிரஸ் வேகத்துல பேசுவா அந்த மெண்டலு.</b-card-text>

                <hr/>

                <b-card-text>அக்கறை (or) பாசம்</b-card-text>
                <b-card-text>என் அம்மாவிற்கு அடுத்தது என் மேல் அளவு கடந்த பாசத்தை வைப்பவளும் அவள் தான்</b-card-text>
                <b-card-text>சண்டை போட்டால் உடனே மன்னிப்பும் கேட்பாள்</b-card-text>
                <b-card-text>என்னை விட அதிகமாக என்னை காதலிக்கிறாள். Means, காதலிப்பதில் எனக்கும் அவளுக்கும் போட்டி வைத்தால் அந்த போட்டியில் அவள் தன் வெற்றி பெறுவாள் 🖤</b-card-text>

                <hr/>

                <b-card-text>சண்டை</b-card-text>
                <b-card-text>சண்டை என்று வந்துவிட்டால், நம் மேல் தவறே இருக்காது, இருந்தாலும் அவள் பேசும் பேச்சுக்கு நாம் செய்தது தான் தவறு என்று நாமே ஒத்துக்கொள்வோம் என்று சொல்லும் அளவிற்கு சண்டை போடுவாள் 😤</b-card-text>
                <b-card-text>வாய் மட்டும் இல்லை என்றால் நாய் கூட அவளை சீண்டாது 😁</b-card-text>
                <b-card-text>அந்த சண்டையை கூட வெட்கமே இல்லாமல் நான் ரசிப்பேன் 😁</b-card-text>

                <hr/>

                <b-card-text>இன்னும் இவளை பற்றி சொல்ல நிறைய இருக்கு.இதுவே போதும் இவளுக்கு😁</b-card-text>

            </b-card>
            </b-card-group>

            <b-card-group deck class="mt-3">
            <b-card
                border-variant="primary"
                header="எங்களின் சந்திப்பு 🖤"
                header-bg-variant="primary"
                header-text-variant="white"
                align="center"
            >
                <b-card-text>இருவரும் சந்திக்கும் போது லவ் அப்படின்ற பீல் இல்லவே இல்லை. ஏனென்றால் இருவரும் நண்பர்கள் போல தான் பேசி வந்தோம். நாங்க ஒரு வருடம் பேசிருப்போம் நல்ல நண்பர்களாகவே.</b-card-text>
                <b-card-text>அந்த முதல் சந்திப்பில் என்னை கலாய்த்து கொண்டே வந்தால். நானும் சிரித்து கொண்டே வந்தேன். அப்பறம் சாப்பிட சென்றோம். அவளுக்கும் எனக்கும் அந்த இடம் புதிது. அப்பவும் என்னை திட்டி கொண்டே வந்தால். உனக்கு ஒரு மண்ணும் தெரில அப்டினு</b-card-text>
                <b-card-text>நானும் என் தலையெழுத்து யாரை விட்டது என்று அவளிடம் சொல்லி கொண்டே சென்றேன் அப்புறம் சிறிய சிரிப்புடன். அவளும் முறைத்து பார்த்தாள். அதற்க்கு அவள் ohh உனக்கு அவ்வளவு ஆகி விட்டதா என்று மறுபடியும் திட்ட ஆரம்பித்தாள். நானும் வாயை திறக்காமல் அவள் பின்னாடியே சென்றேன் சாப்பாடு சாப்பிட</b-card-text>
                <b-card-text>பிறகு இருவரும் கடற்கரைக்கு சென்றோம். அங்கு சிறிது நேரம் பேசி விட்டு பிறகு அங்கிருந்து சென்றோம். அப்புறம் அவளை அவள் தங்கும் அறையில் விட்டு விட்டு சென்றேன்</b-card-text>
                <b-card-text>அதன் பின்னரும் இருவரும் சந்தித்தோம். அப்படியே பேசி பேசி அவளிடம் மாட்டிக்கொண்டேன். Means, காதலில் விழுந்து விட்டோம்.</b-card-text>
                <b-card-text>இன்னும் சொல்வதற்கு நிறைய இருக்கு. பட் அதெல்லாம் சொன்ன நல்ல இருக்காது, Because, it's our personal 😘😍</b-card-text>
            </b-card>
            </b-card-group>
        
            <b-card-group deck class="mt-3">
            <b-card
                border-variant="primary"
                header="இது என் கண்மணிக்காக 🖤"
                header-bg-variant="primary"
                header-text-variant="white"
                align="center"
            >
                <b-card-text>ஆளு பாக்கவே நல்லா கருவண்டு மாதிரி இருப்பா 😘😍. ஆனா நாங்க போட்டோ எடுக்கும் போது அவ மட்டும் நல்லா வெள்ளையா தெரிவா. இருந்தாலும் அவ என் கண்மணி தான் 😍</b-card-text>
                <b-card-text>பாக்கவே ஓணான் மாதிரி இருப்பா. அவ்ளோ ஒள்ளிய இருப்பா. என்னமோ பஞ்சத்துல அடி பட்டவ மாதிரி 😁</b-card-text>
                <b-card-text>நல்லா பேசுவா. அவ என் கூட இருக்கும் போது எந்த கஷ்டமும் எனக்கு தெரியாது. காதல் கண்ணை மறைக்கும் னு சொல்லுவாங்களா அது இது தான் போல.</b-card-text>
                <b-card-text>அவ கூட பேசுனது பழகுனத ல நெனச்சாலே எவ்ளோ சோகமா இருந்தாலும் என்னை அறியாமலே சிரிச்சிருவேன்.</b-card-text>
                <b-card-text>ஏன் இப்போ இந்த website haa develope பண்றதுகு காரணமும் அவ மேல இருக்க இந்த லவ் தான் 🖤</b-card-text>
                <b-card-text>அவளை விட அவ கன்னத்துக்கு கீழே இருக்க மச்சம் தான் எனக்கு ரொம்ப புடிக்கும் 😍</b-card-text>
                <b-card-text>வாரத்துக்கு ஒரு முறை ஆவது அவ கூட time ஸ்பென்ட் பண்ணனும் னு தோணும்</b-card-text>
            </b-card>
            </b-card-group>
        
            <b-card-group deck class="mt-3">
            <b-card
                border-variant="primary"
                header="அவளுக்கான கவிதை"
                header-bg-variant="primary"
                header-text-variant="white"
                align="center"
            >
                <b-card-text>எங்கேயும் எப்போதும் யாருக்காகவும் விட்டு கொடுக்க முடியாத ஓர் உறவு என்றால் அது நீ மட்டுமே என் கண்மணி 🖤🖤🖤</b-card-text>
            </b-card>
            </b-card-group>
        
            <b-card-group deck class="mt-3">
            <b-card
                border-variant="primary"
                header="கடைசியாக"
                header-bg-variant="primary"
                header-text-variant="white"
                align="center"
            >
                <b-card-text>I hate You 🖤🖤🖤 KANMANI</b-card-text>
            </b-card>
            </b-card-group>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'FBody-Component',
        data(){
            return({
                show_hide_div: false
            })
        }
    }
</script>