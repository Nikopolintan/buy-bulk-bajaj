<script setup>
import AppLayout from '@/components/layout/AppLayout.vue'
import LoginForm from '@/components/auth/LoginForm.vue'

</script>

<template>
  <AppLayout>
    <template #content>
      <v-row class="my-auto">
        <v-col cols="12" class="mx-auto">
          <v-card class="mx-auto text-center border rounded-lg pa-4" width="400" elevation="15">
            <v-card-title class="d-flex flex-column align-center">
              <v-img src="/images/BULKBUY logo.png" width="120" height="120"></v-img>
              <h4 class="font-weight-black">BULKBUY</h4>
              <small><i>bajaj and budget</i></small>
              <!-- Login Buttons -->
              <div class="d-flex justify-center gap-2 mt-1">
                <a
                  href="https://accounts.google.com/v3/signin/identifier?continue=https%3A%2F%2Fmail.google.com%2Fmail%2Fu%2F0%2F&emr=1&followup=https%3A%2F%2Fmail.google.com%2Fmail%2Fu%2F0%2F&ifkv=AXH0vVv1aZquQkKy1DvX7LazCQyITaqv1whhreqNO1DziAMumtmDbQiIkIjKri3LtaMcLKfSgMy6&osid=1&passive=1209600&service=mail&flowName=GlifWebSignIn&flowEntry=ServiceLogin&dsh=S1259117950%3A1744073433066288"
                  target="_blank"
                >
                  <v-img src="/images/googlelogo.png" width="50" height="50"></v-img>
                </a>

                <a class="mt-2" href="https://web.facebook.com/?_rdc=1&_rdr#" target="_blank">
                  <v-img src="/images/fblogo.png" width="35" height="35" class="mx-2"></v-img>
                </a>
              </div>
              <small>——————— or ———————
              </small>
            </v-card-title>

            <v-card-text class="pt-2">
              <v-sheet class="mx-auto" width="300">

                <LoginForm></LoginForm>

              </v-sheet>
              <v-divider class="mt-3"></v-divider>
              <h5 class="mt-2">
                Don't have an account?
                <RouterLink class="text-primary" to="/register">Click to Register</RouterLink>
              </h5>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </template>
  </AppLayout>
</template>

<style scoped>
/* Apply Poppins font*/
body {
  font-family: 'Poppins', sans-serif;
}

.v-app-bar,
.v-card,
.v-card-text,
.v-btn {
  font-family: 'Poppins', sans-serif; /* Ensures components use Poppins */
}
</style>
