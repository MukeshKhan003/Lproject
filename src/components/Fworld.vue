<template>
    <div>
        
        <div>
            <b-card :title="card_header">
                <b-card-text>
                    யார் அந்த கண்மணி ?
                </b-card-text>

                <b-card-text>அவளுக்காக மட்டும் தான் இந்த Website<b-icon icon="heart-fill" font-scale="1.5"></b-icon></b-card-text>
                
                <b-button :disabled="fbody_comp_enable ? true : false"  @click="verifyFunc()">Verify</b-button>
            </b-card>
        </div>

        <b-alert
            :show="dismissCountDown"
            dismissible
            :variant="alert_color"
            @dismissed="dismissCountDown=0"
            @dismiss-count-down="countDownChanged"
            >
            {{ success_alert}}
            {{ error_alert }} {{ dismissCountDown }} seconds...
        </b-alert>

        <div>
            <b-card class="mt-5" v-if="show_number_content">
                <div role="group">
                    <label for="input-live">PH NO:</label>
                    <b-form-input
                    type="number"
                    id="input-live"
                    v-model="phone_number"
                    :state="nameState"
                    aria-describedby="input-live-help input-live-feedback"
                    placeholder="Enter Phone Number"
                    trim
                    ></b-form-input>

                    <!-- This will only be shown if the preceding input has an invalid state -->
                    <b-form-invalid-feedback id="input-live-feedback">
                    Enter at least 10 letters
                    </b-form-invalid-feedback>
                    
                    <label class="mt-3" for="input-live">Enter First Meetup Date:</label>
                    <b-form-input
                    type="date"
                    id="input-live"
                    v-model="first_meetup_date"
                    aria-describedby="input-live-help input-live-feedback"
                    trim
                    ></b-form-input>

                    <label class="mt-3" for="input-live">Enter Un aalu Number</label>
                    <b-form-input
                    type="number"
                    id="input-live"
                    v-model="darling_number"
                    :state="nameState"
                    aria-describedby="input-live-help input-live-feedback"
                    placeholder="Enter Your allu Number"
                    trim
                    ></b-form-input>

                    <b-button class="mt-3" variant="success" @click="verify_details()">Verify Your Details</b-button>
                </div>
            </b-card>
        </div>

        <Fbody v-if="fbody_comp_enable && dismissCountDown == 0"/>
    </div>
</template>

<script>
import Fbody from './Fbody.vue'
export default {
    name: "Fworld-Mworld",
    components: { Fbody },
    data(){
        return({
            card_header: "கண்மணி",
            show_number_content: false,
            phone_number: '',
            first_meetup_date: '',
            darling_number: '',
            original_phone_number: 8903785633,
            original_meetup_date: '2022-09-04',
            original_darling_number: 8525844231,
            dismissSecs: 5,
            dismissCountDown: 0,
            error_alert: '',
            success_alert: '',
            alert_color: 'danger',
            fbody_comp_enable: false
        })
    },
    computed: {
      nameState() {
        return this.phone_number.length > 9 ? true : false
      }
    },
    methods: {
        verifyFunc: function() {
            this.show_number_content = true;
        },
        verify_details: function() {
            console.log("Event Enter");
            if(this.original_phone_number != this.phone_number){
                this.error_alert = "Phone number haa correct haa enter pannu d venna"
                this.dismissCountDown = this.dismissSecs;
                return;
            }

            if(this.original_meetup_date !== this.first_meetup_date){
                this.error_alert = "Oru date koodava d niyabagam vechika mata"
                this.dismissCountDown = 10;
                return;
            }
            
            if(this.darling_number != this.original_darling_number){
                this.error_alert = "Un Aaalu Phone number koodava d niyabagam vechika mata.. Thiruttu maadu"
                this.dismissCountDown = 10;
                return;
            }

            this.alert_color = "success";
            this.error_alert = "";
            this.success_alert = "சூப்பர் டீ. உன்னை நினைத்து பெருமை படுகிறேன் 😊";
            this.dismissCountDown = 10;

            this.show_number_content = false;
            this.fbody_comp_enable = true;
        },
        countDownChanged(dismissCountDown) {
            this.dismissCountDown = dismissCountDown
        }
    }
}
</script>
