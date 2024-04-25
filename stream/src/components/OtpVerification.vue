<script setup>
import 'typeface-poppins'
import FooterLink from './FooterLink.vue'
import MainLogo from './MainLogo.vue'
import googlelogo from '@/assets/images/google-logo.png'
import appleLogo from '@/assets/images/apple-logo.png'
import { useRouter } from 'vue-router'

// Function to navigate to sign-in page
const navigateToSignIn = () => {
  const router = useRouter()
  router.push('/signin') // Navigate to /signin route
}
</script>

<template>
  <div class="container d-flex align-items-center justify-content-between flex-column vh-100">
    <MainLogo />
    <div class="row justify-content-center align-items-center maincontent w-100">
      <div class="col-xl-6 col-lg-7 col-md-10 col-12">
        <h1 class="welcome-title text-center">Check your email for a code</h1>
        <h3 class="element-text">
          We've sent a 6-character code to john_brown@company.com The code expires shortly, so
          please enter it soon.
        </h3>

        <div class="sign-in-detail-wrapper">
          <div class="otp-number d-flex align-items-center justify-content-between mb-4">
            <div>
              <input type="text" name="" id="" />
            </div>
            <div>
              <input type="text" name="" id="" />
            </div>
            <div>
              <input type="text" name="" id="" />
            </div>
            <div>
              <input type="text" name="" id="" />
            </div>
            <div>
              <input type="text" name="" id="" />
            </div>
          </div>
          <router-link to="/signin" class="element-btn w-100 mb-4 mt-2">Continue</router-link>.
          <!-- <button class="element-btn w-100 mb-4 mt-2" @click="navigateToSignIn">Continue</button> -->
          <h3 class="element-text mb-0 mt-3">
            Didn't get and SMS?
            <router-link to="" class="sign-In-manually">Send again</router-link>.
          </h3>
          <h3 class="element-text mb-0 mt-5">Can't find your code? Check your spam folder!</h3>
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
.otp-number input {
  height: 72px;
  border-radius: 8px;
  border: 1px solid #d4e1e4;
  outline: none;
  width: 72px;
  text-align: center;
}
.element-btn {
  border: none;
  padding: 15px 16px 15px 16px;
  border-radius: 8px;
  font-family: 'Poppins', sans-serif;
  background-color: #3cc553;
  color: #fff;
  display: block;
  width: 100%;
  text-align: center;
  text-decoration: none;
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
