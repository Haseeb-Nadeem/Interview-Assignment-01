<script setup>
import 'typeface-poppins'
import MainLogo from './MainLogo.vue'
import homeIcon from '@/assets/images/home_icon.png'
import Bell from '@/assets/images/Bell.png'
import GearSix from '@/assets/images/GearSix.png'
import QuestionHead from '@/assets/images/Questionhead.png'
import Avatar from '@/assets/images/avatar.png'
import FrameDots from '@/assets/images/Frame-dots.png'
import MagnifyingGlass from '@/assets/images/MagnifyingGlass.png'
import mainLogo from '@/assets/images/main-logo.png'
import FrameUser from '@/assets/images/Frame-user.png'
import Frame from '@/assets/images/Frame.png'
import AddUser from '@/assets/images/add-user.png'
import SettingIcon from '@/assets/images/setting-icon.png'
import WorkingStatus from './WorkingStatus.vue'
</script>

<template>
  <header>
    <div class="container-fluid border-bottom">
      <div class="header-wrap d-flex align-items-center justify-content-between">
        <section class="d-flex align-items-center">
          <div class="home-page-logo">
            <router-link to="/" class="sign-In-manually">
              <img :src="mainLogo" alt="main Logo" class="img-fluid" />
            </router-link>
          </div>
          <div
            class="d-xxl-flex d-xl-flex d-lg-flex d-md-none d-none align-items-center website-icons-link border-left gap-2"
          >
            <img :src="homeIcon" alt="" />
            <select
              class="form-select custom-form-select form-select-lg p-0 border-0"
              aria-label=".form-select-lg example"
            >
              <option selected>PMS HUB/HOME</option>
              <option value="1">One</option>
              <option value="2">Two</option>
              <option value="3">Three</option>
            </select>
          </div>
        </section>

        <section class="d-flex align-items-center">
          <div class="website-icons-link">
            <div class="search-br-wrap">
              <img :src="MagnifyingGlass" alt="MagnifyingGlass" />
              <input type="text" placeholder="Search anything" class="border-0" />
            </div>
          </div>

          <div
            class="website-icons-link border-right border-left d-flex align-items-center justify-content-between"
          >
            <router-link to="#" class="sign-In-manually d-xxl-none d-xl-none d-lg-none d-md-none">
              <img :src="MagnifyingGlass" alt="MagnifyingGlass" />
            </router-link>
            <router-link to="#" class="sign-In-manually">
              <img :src="Bell" alt="Bell" />
            </router-link>
            <router-link to="#" class="sign-In-manually">
              <img :src="QuestionHead" alt="QuestionHead" />
            </router-link>
            <router-link to="#" class="sign-In-manually">
              <img :src="GearSix" alt="GearSix" />
            </router-link>
          </div>
          <div
            class="website-icons-link border-right pe-0 d-flex align-items-center justify-content-between"
          >
            <router-link to="#" class="sign-In-manually">
              <img :src="FrameDots" alt="FrameDots" />
            </router-link>
            <router-link to="#" class="sign-In-manually">
              <img :src="Avatar" alt="Avatar" />
            </router-link>
          </div>
        </section>
      </div>
    </div>

    <div class="container-fluid">
      <div class="d-flex align-items-center mt-3 gap-2 d-xxl-none d-xl-none d-lg-none d-md-flex">
        <img :src="homeIcon" alt="" />
        <select
          class="form-select custom-form-select form-select-lg p-0 border-0"
          aria-label=".form-select-lg example"
        >
          <option selected>PMS HUB/HOME</option>
          <option value="1">One</option>
          <option value="2">Two</option>
          <option value="3">Three</option>
        </select>
      </div>
      <section class="total-criteria-wrapper mt-3">
        <div class="card-wrapper">
          <div class="card-criteria d-flex align-items-center gap-3 mb-3">
            <span class="element-text">Total Project</span>
            <div class="d-flex align-items-center gap-1 accesding-list">
              <i class="fa fa-caret-up" aria-hidden="true"></i>
              <span class="element-text">2</span>
            </div>
          </div>
          <h3 class="project-number mb-0">7</h3>
        </div>
        <div class="card-wrapper">
          <div class="card-criteria d-flex align-items-center gap-3 mb-3">
            <span class="element-text">Total Task</span>
            <div class="d-flex align-items-center gap-1 accesding-list">
              <i class="fa fa-caret-up" aria-hidden="true"></i>
              <span class="element-text">4</span>
            </div>
          </div>
          <h3 class="project-number mb-0">49</h3>
        </div>
        <div class="card-wrapper">
          <div class="card-criteria d-flex align-items-center gap-3 mb-3">
            <span class="element-text">Assigned Task</span>
            <div class="d-flex align-items-center gap-1 descending-list">
              <i class="fa fa-caret-down" aria-hidden="true"></i>
              <span class="element-text">3</span>
            </div>
          </div>
          <h3 class="project-number mb-0">12</h3>
        </div>
        <div class="card-wrapper">
          <div class="card-criteria d-flex align-items-center gap-3 mb-3">
            <span class="element-text">Completed Task</span>
            <div class="d-flex align-items-center gap-1 accesding-list">
              <i class="fa fa-caret-up" aria-hidden="true"></i>
              <span class="element-text">1</span>
            </div>
          </div>
          <h3 class="project-number mb-0">6</h3>
        </div>
        <div class="card-wrapper">
          <div class="card-criteria d-flex align-items-center gap-3 mb-3">
            <span class="element-text">Overdue Tasks</span>
            <div class="d-flex align-items-center gap-1 descending-list">
              <i class="fa fa-caret-down" aria-hidden="true"></i>
              <span class="element-text">2</span>
            </div>
          </div>
          <h3 class="project-number mb-0">3</h3>
        </div>
      </section>
      <section class="working-dashbaord mt-3 mb-5">
        <div class="hirarchy-board d-flex align-items-center justify-content-between">
          <div class="filteration d-flex align-items-center gap-4">
            <div class="d-flex align-items-center gap-3">
              <div class="user-list d-flex align-items-center">
                <a href="#">
                  <img :src="FrameUser" alt="FrameUser" />
                </a>
                <a href="#">
                  <img :src="Frame" alt="FrameUser" />
                </a>
              </div>
              <div class="add-user">
                <a href="#">
                  <img :src="AddUser" alt="AddUser" />
                </a>
              </div>
            </div>

            <div class="select-filter d-flex align-items-center">
              <select
                class="form-select custom-form-select form-select-lg p-0 border-0"
                aria-label=".form-select-lg example"
              >
                <option selected>Status catagory</option>
                <option value="1">One</option>
                <option value="2">Two</option>
                <option value="3">Three</option>
              </select>
              <select
                class="form-select custom-form-select form-select-lg p-0 border-0"
                aria-label=".form-select-lg example"
              >
                <option selected>Workspaces</option>
                <option value="1">One</option>
                <option value="2">Two</option>
                <option value="3">Three</option>
              </select>
              <select
                class="form-select custom-form-select form-select-lg p-0 border-0"
                aria-label=".form-select-lg example"
              >
                <option selected>Quick filter</option>
                <option value="1">One</option>
                <option value="2">Two</option>
                <option value="3">Three</option>
              </select>
            </div>
          </div>
          <div class="view-setting-btn">
            <router-link to="" class="setting-btn">
              <img :src="SettingIcon" alt="SettingIcon" />
              View Settings</router-link
            >
          </div>
        </div>

        <WorkingStatus />
      </section>
    </div>
  </header>
</template>

<style scoped>
.working-dashbaord {
  border: 1px solid #d4e1e4;
  border-radius: 8px;
  padding: 16px;
}
.hirarchy-board {
  border-bottom: 1px dashed #95acaa;
  padding-bottom: 12px;
}
.total-criteria-wrapper {
  border: 1px solid #d4e1e4;
  border-radius: 14px;
  padding: 16px 10px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.header-wrap {
  padding: 10px 0px;
}
.custom-form-select {
  font-size: 16px;
  font-weight: 500;
  padding-right: 36px !important;
  width: auto;
}
.card-wrapper {
  border-right: 1px dashed #95acaa;
  padding: 12px 20px 12px 20px;
  width: 20%;
}
.card-wrapper:last-child {
  border-right: 0px;
}
.custom-form-select:focus {
  border-color: unset !important;
  outline: 0;
  box-shadow: unset !important;
}
.project-number {
  font-family: 'Poppins', sans-serif;
  font-size: 28px;
  font-weight: 600;
  line-height: 32px;
}
.home-page-logo img {
  height: 36px;
  padding-right: 20px;
}
.user-list a:first-child {
  display: block;
  margin-left: 0px;
}
.user-list a:first-child img {
  position: relative;
  z-index: 99;
}
.user-list a {
  display: block;
  margin-left: -10px;
}
.accesding-list i,
.accesding-list span {
  color: #2cc171;
}
.descending-list i,
.descending-list span {
  color: #e27233;
}
.search-br-wrap {
  border: 1px solid #d4e1e4;
  background-color: #f4f8f9;
  border-radius: 8px;
  padding: 8px 8px 8px 14px;
}
.search-br-wrap input {
  outline: 0;
  background-color: transparent;
  font-size: 16px;
  font-weight: 400;
  line-height: 22px;
  padding-left: 10px;
}
.search-br-wrap input::placeholder {
  color: #d4e1e4;
}
.setting-btn {
  background: #f1f2f4;
  border-radius: 8px;
  padding: 4px 8px 4px 8px;
  text-decoration: none;
  color: #4f4f4f;
  font-weight: 500;
  font-size: 16px;
  line-height: 22px;
  display: flex;
  align-items: center;
  gap: 10px;
}
.element-text {
  font-family: 'Poppins', sans-serif;
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  text-align: center;
}
.website-icons-link {
  padding: 0px 20px;
  gap: 20px;
}
.border-bottom {
  border-bottom: 1px solid #d4e1e4;
}
.border-right {
  border-right: 1px solid #d4e1e4;
}
.border-left {
  border-left: 1px solid #d4e1e4;
}
.border-right:last-child {
  border-right: 0px;
}

@media (max-width: 991px) {
  .element-text {
    font-family: 'Poppins', sans-serif;
    font-size: 12px;
    font-weight: 400;
    line-height: 24px;
    text-align: center;
  }
  .project-number {
    font-family: 'Poppins', sans-serif;
    font-size: 22px;
    font-weight: 600;
    line-height: 32px;
  }
  .card-wrapper {
    border-right: 1px dashed #95acaa;
    padding: 12px 10px 12px 10px;
    width: 20%;
  }
}

@media (max-width: 767px) {
  .card-wrapper {
    border-right: none;
    padding: 12px 20px 12px 20px;
    width: 48%;
    border-bottom: 1px dashed #95acaa;
  }
  .card-wrapper:last-child {
    border-right: none;
    border-bottom: none;
  }
  .total-criteria-wrapper {
    border: 1px solid #d4e1e4;
    border-radius: 14px;
    padding: 16px 10px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
  }
  .hirarchy-board {
    border-bottom: 1px dashed #95acaa;
    padding-bottom: 12px;
    flex-wrap: wrap;
  }
  .filteration {
    width: 100%;
    margin-bottom: 20px;
    flex-wrap: wrap;
  }
  .view-setting-btn {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: end;
  }
  .select-filter {
    width: 100%;
    flex-wrap: wrap;
    gap: 10px;
  }
  .search-br-wrap {
    border: 1px solid #d4e1e4;
    background-color: #f4f8f9;
    border-radius: 8px;
    padding: 8px 8px 8px 14px;
    display: none;
  }
}
@media (max-width: 575px) {
  .total-criteria-wrapper {
    border: 1px solid #d4e1e4;
    border-radius: 14px;
    padding: 16px 10px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
  }
  .card-wrapper {
    border-right: none;
    padding: 12px 20px 12px 20px;
    width: 100%;
    border-bottom: 1px dashed #95acaa;
  }
  .card-wrapper:last-child {
    border-bottom: none;
  }
}

@media (max-width: 480px) {
  .website-icons-link {
    padding: 0px 15px 0px 0px;
    gap: 10px;
  }
  .border-left {
    border-left: 0px;
  }
  .border-right {
    border-right: 0px;
  }
}
</style>
