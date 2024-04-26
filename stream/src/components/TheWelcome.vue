<script setup>
import { ref } from 'vue'

// Define the email ref
const email = ref('')
const isAutofilled = ref(false)

// Define the method to check autofill
const checkAutofill = (event) => {
  // Check if input value is autofilled
  isAutofilled.value = event.target.value !== ''
}
import 'typeface-poppins'
import FooterLink from './FooterLink.vue'
import MainLogo from './MainLogo.vue'
import googlelogo from '@/assets/images/google-logo.png'
import appleLogo from '@/assets/images/apple-logo.png'
</script>

<template>
  <div class="container d-flex align-items-center justify-content-between flex-column vh-100">
    <MainLogo />
    <div class="row justify-content-center align-items-center maincontent w-100">
      <div class="col-xl-6 col-lg-7 col-md-10 col-12">
        <h1 class="welcome-title text-center">Hi, Welcome Back to Streamed!</h1>
        <h3 class="element-text">We suggest using the email address that you use at work.</h3>

        <div class="sign-in-detail-wrapper">
          <div class="googl-links-wrap">
            <router-link to="/otp" class="signIn-social-icon mb-3"
              ><img :src="googlelogo" alt="Google Logo" /> Continue with Google</router-link
            >
            <router-link to="/otp" class="signIn-social-icon mb-3"
              ><img :src="appleLogo" alt="Google Logo" /> Continue with Apple</router-link
            >
          </div>

          <div class="or-text d-flex align-items-center justify-content-center gap-2 mb-3">
            <h6 class="mb-0"></h6>
            <p class="choice-text text-center mb-0">OR</p>
            <h6 class="mb-0"></h6>
          </div>

          <div class="mb-4">
            <label for="" class="element-text pb-1">Your Email</label>
            <input
              type="email"
              name="email"
              id="email"
              autocomplete="email"
              class="email-input w-100 text-left"
              placeholder="e.g. john_brown@company.com"
              required
              @input="checkAutofill"
              v-model="email"
            />
          </div>
          <router-link
            to="/otp"
            :class="{ 'element-btn': true, autofilled: isAutofilled }"
            class="element-btn w-100 mb-4"
            >Continue</router-link
          >
          <h3 class="element-text card-bg-theme mb-0">
            We'll email you a magic code for a password-free sign-in. Or you can
            <router-link to="" class="sign-In-manually">sign in manually instead</router-link>.
          </h3>
        </div>
      </div>
    </div>
    <div class="row justify-content-center align-items-center w-100">
      <div class="col-md-6">
        <div class="footer-wrapper">
          <FooterLink />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.maincontent {
  margin: 90px 0px;
}
.sign-in-detail-wrapper {
  padding: 50px 55px 0px 55px;
}
.welcome-title {
  font-family: 'Poppins', sans-serif;
  font-size: 32px;
  font-weight: 700;
  line-height: 48px;
}
.element-text {
  font-family: 'Poppins', sans-serif;
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  text-align: center;
}
.signIn-social-icon {
  border: 1px solid #d4e1e4;
  padding: 15px 16px 15px 16px;
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  color: #101010;
  font-size: 16px;
  font-weight: 400;
  gap: 12px;
  font-family: 'Poppins', sans-serif;
}
.or-text h6 {
  border-top: 1px solid #d4e1e4;
  width: 100%;
}
.email-input {
  border: 1px solid #d4e1e4;
  padding: 15px 16px 15px 16px;
  border-radius: 8px;
  outline: none;
  font-family: 'Poppins', sans-serif;
}
.email-input::placeholder {
  color: #d4e1e4;
}

.element-btn {
  border: none;
  padding: 15px 16px 15px 16px;
  border-radius: 8px;
  font-family: 'Poppins', sans-serif;
  background-color: #3cc55380;
  color: #fff;
  display: block;
  width: 100%;
  text-align: center;
  text-decoration: none;
}

.autofilled {
  border: none;
  padding: 15px 16px 15px 16px;
  border-radius: 8px;
  font-family: 'Poppins', sans-serif;
  color: #fff;
  display: block;
  width: 100%;
  text-align: center;
  text-decoration: none;
  background-color: #3cc553;
}
.element-text.card-bg-theme {
  background-color: #f4f8f9;
  font-size: 16px;
  font-weight: 400;
  font-family: 'Poppins', sans-serif;
  line-height: 22px;
  padding: 12px;
  border-radius: 8px;
  text-align: left;
}
.sign-In-manually {
  color: #3cc553;
  font-size: 16px;
  font-weight: 500;
  font-family: 'Poppins', sans-serif;
  line-height: 22px;
  text-decoration: none;
}
.footer-wrapper {
  padding: 0px 55px 0px 55px;
}

@media (min-width: 1400px) {
  .sign-in-detail-wrapper {
    padding: 50px 100px 0px 100px;
  }
  .footer-wrapper {
    padding: 0px 100px 0px 100px;
  }
}

@media (max-width: 767px) {
  .welcome-title {
    font-family: 'Poppins', sans-serif;
    font-size: 26px;
    font-weight: 700;
    line-height: 34px;
  }
  .element-text {
    font-family: 'Poppins', sans-serif;
    font-size: 14px;
    font-weight: 400;
    line-height: 24px;
    text-align: center;
  }
  .footer-text {
    font-family: 'Poppins', sans-serif;
    font-size: 14px;
    font-weight: 400;
    line-height: 20px;
    text-align: center;
  }
  .element-text.card-bg-theme {
    background-color: #f4f8f9;
    font-size: 14px;
    font-weight: 400;
    font-family: 'Poppins', sans-serif;
    line-height: 22px;
    padding: 12px;
    border-radius: 8px;
    text-align: left;
  }
}

@media (max-width: 480px) {
  .sign-in-detail-wrapper {
    padding: 50px 0px 0px 0px;
  }
  .footer-wrapper {
    padding: 0px 10px 0px 10px;
  }
}
</style>
