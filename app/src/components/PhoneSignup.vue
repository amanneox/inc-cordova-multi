<<<<<<< HEAD
<template><div id="app">
  <v-app id="inspire">
    <v-content>
      <v-container fluid fill-height>
        <v-layout align-center justify-center>
          <v-flex xs12 sm8 md4>
            <v-card class="elevation-10">
              <v-toolbar dark color="primary">
                <v-toolbar-title>Aapki Seva Mein</v-toolbar-title>
                <v-spacer></v-spacer>
                <v-tooltip bottom>
                  <v-btn
                    icon
                    large
                    :href="Help"
                    target="_blank"
                    slot="activator"
                  ><v-icon large>help</v-icon>
                  </v-btn>
                  <span>Help</span>
                </v-tooltip>
              </v-toolbar>
              <v-card-text>
                <v-form>
                  <v-flex xs12>
            <v-text-field
              value="Phone No."
               readonly
            ></v-text-field>
          </v-flex>
                 <v-flex>
                    <v-text-field
                    prepend-inner-icon="call"
                    type="number"
                    label="Enter your No. here"
                    single-line
                    outline
                    v-model = "phone"
                    :rules="phoneRules"
                    ></v-text-field>
                  </v-flex>
                 <v-card-actions>
                  <v-btn
                  large
                  depressed
                  block
                  color="primary"
                  >Submit</v-btn>
                </v-card-actions>
              </v-form>
            </v-card-text>
           </v-card>
        </v-flex>
      </v-layout>
    </v-container>
  </v-content>
</v-app>
</div></template>
=======
<template>
  <v-container pa-0>
    <v-layout>
      <v-container grid-list>
        <v-card>
          <v-card-text>
            <v-form>
              <div style="margin-bottom: 10px;">
                <span style="font-size: 20px; color: blue">Phone Number</span>
              </div>
              <v-text-field
                type="number"
                label="Enter your Number here"
                single-line outline v-model="phone"
                v-validate="`required|digits:10`">
              </v-text-field>
              <v-card-actions>
                <v-btn large outline block color="primary">Submit</v-btn>
              </v-card-actions>
            </v-form>
          </v-card-text>
        </v-card><br/>
        <v-card>
          <v-card-text>
            <v-form>
              <div style="margin-bottom: 10px">
                <span style="font-size: 20px; color: blue;">Enter OTP</span>
              </div>
              <v-text-field
                label="OTP"
                type="number"
                single-line
                outline
                v-validate="`required|digits:4`">
              </v-text-field>
              <v-card-actions>
                <v-btn large outline block color="primary">Confirm OTP</v-btn>
              </v-card-actions>
            </v-form>
          </v-card-text>
        </v-card>
      </v-container>
    </v-layout>
  </v-container>
</template>
>>>>>>> b21869275486db53d5ae5f2e53049f46a5c3eb2a
<script>
  export default {
    data () {
      return {
<<<<<<< HEAD
        email: '',
        password: '',
        phone: '',
        phoneRules: [
          v => !!v || 'Phone is required',
          v => v.length === 10 || 'Enter valid number'
        ],
        rules: {
          required: value => !!value || 'Required.',
          email: v => /.+@.+/.test(v) || 'E-mail must be valid'
        }
=======
>>>>>>> b21869275486db53d5ae5f2e53049f46a5c3eb2a
      }
    },
    computed: {
    }
  }
  </script>
