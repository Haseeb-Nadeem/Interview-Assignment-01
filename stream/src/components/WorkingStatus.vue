<script setup>
import PlusSign from '@/assets/images/plus-sign.png'
import Image16 from '@/assets/images/image-16.png'
import Ellipse5 from '@/assets/images/Ellipse-5.png'
import Ellipse4 from '@/assets/images/Ellipse-4.png'
import MinusSign from '@/assets/images/minus-sign.png'
</script>

<template>
  <div class="table-responsive working-status-tble-wrap mt-3">
    <table class="table working-status-tble mb-0">
      <tr>
        <th style="width: 35%"></th>
        <th>JAN</th>
        <th>FEB</th>
        <th>MAR</th>
      </tr>
      <tr>
        <td>
          <div class="d-flex p-0 align-items-center bg-transparent justify-content-between">
            <div class="d-flex align-items-center gap-2">
              <a href="#">
                <img :src="PlusSign" alt="PlusSign" />
              </a>
              <h6 class="mb-0">My Hive</h6>
            </div>
            <div>
              <router-link to="/" class="assign-user">
                <img :src="Image16" alt="Image16" class="img-fluid" />
              </router-link>
              <router-link to="/" class="assign-user">
                <img :src="Ellipse4" alt="Ellipse4" class="img-fluid" />
              </router-link>
              <router-link to="/" class="assign-user">
                <img :src="Ellipse5" alt="Ellipse5" class="img-fluid" />
              </router-link>
            </div>
          </div>
        </td>
        <td colspan="3">
          <div class="progress custom-progress-bar">
            <div
              class="progress-bar"
              role="progressbar"
              style="width: 30%"
              aria-valuenow="30"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
        </td>
      </tr>

      <tr>
        <td>
          <div class="d-flex align-items-center p-0 bg-transparent justify-content-between">
            <div class="d-flex align-items-center gap-2">
              <a href="#">
                <img :src="PlusSign" alt="PlusSign" />
              </a>
              <h6 class="mb-0">Bomjour</h6>
            </div>
            <div>
              <router-link to="/" class="assign-user">
                <img :src="Image16" alt="Image16" class="img-fluid" />
              </router-link>
              <router-link to="/" class="assign-user">
                <img :src="Ellipse4" alt="Ellipse4" class="img-fluid" />
              </router-link>
              <router-link to="/" class="assign-user">
                <img :src="Ellipse5" alt="Ellipse5" class="img-fluid" />
              </router-link>
            </div>
          </div>
        </td>
        <td colspan="3">
          <div class="progress custom-progress-bar">
            <div
              class="progress-bar"
              role="progressbar"
              style="width: 75%"
              aria-valuenow="75"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
        </td>
      </tr>

      <tr>
        <td>
          <div
            class="sub-title d-flex align-items-center p-0 bg-transparent justify-content-between"
          >
            <div class="d-flex align-items-center gap-2">
              <a href="#">
                <img :src="MinusSign" alt="MinusSign" />
              </a>
              <h6 class="mb-0">Candidate</h6>
            </div>
            <div>
              <router-link to="/" class="assign-user">
                <img :src="Ellipse5" alt="Ellipse5" class="img-fluid" />
              </router-link>
            </div>
          </div>
        </td>
        <td colspan="3">
          <div class="progress custom-progress-bar">
            <div
              class="progress-bar"
              role="progressbar"
              style="width: 35%"
              aria-valuenow="35"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
        </td>
      </tr>

      <tr>
        <td>
          <div
            class="d-flex Nested-sub-title align-items-center p-0 bg-transparent justify-content-between"
          >
            <div class="d-flex align-items-center gap-2">
              <a href="#">
                <img :src="MinusSign" alt="MinusSign" />
              </a>
              <h6 class="mb-0">Milestone 1</h6>
            </div>
          </div>
        </td>
        <td colspan="3">
          <div class="progress custom-progress-bar">
            <div
              class="progress-bar"
              role="progressbar"
              style="width: 20%"
              aria-valuenow="20"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
        </td>
      </tr>

      <tr>
        <td>
          <div
            class="d-flex Multi-Nested-sub-title align-items-center p-0 bg-transparent justify-content-between"
          >
            <div class="d-flex align-items-center gap-2">
              <h6 class="mb-0">Authentication</h6>
            </div>
          </div>
        </td>
        <td colspan="3">
          <div class="progress custom-progress-bar">
            <div
              class="progress-bar"
              role="progressbar"
              style="width: 25%"
              aria-valuenow="25"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
        </td>
      </tr>

      <tr>
        <td>
          <div
            class="d-flex Multi-Nested-sub-title align-items-center p-0 bg-transparent justify-content-between"
          >
            <div class="d-flex align-items-center gap-2">
              <h6 class="mb-0">Explore</h6>
            </div>
          </div>
        </td>
        <td colspan="3">
          <div class="progress custom-progress-bar">
            <div
              class="progress-bar"
              role="progressbar"
              style="width: 15%"
              aria-valuenow="15"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
        </td>
      </tr>

      <tr>
        <td>
          <div
            class="d-flex Nested-sub-title align-items-center p-0 bg-transparent justify-content-between"
          >
            <div class="d-flex align-items-center gap-2">
              <a href="#">
                <img :src="PlusSign" alt="PlusSign" />
              </a>
              <h6 class="mb-0">Milestone 2</h6>
            </div>
          </div>
        </td>
        <td colspan="3">
          <div class="progress custom-progress-bar">
            <div
              class="progress-bar"
              role="progressbar"
              style="width: 5%"
              aria-valuenow="5"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
        </td>
      </tr>

      <tr>
        <td>
          <div
            class="sub-title d-flex align-items-center p-0 bg-transparent justify-content-between"
          >
            <div class="d-flex align-items-center gap-2">
              <a href="#">
                <img :src="PlusSign" alt="PlusSign" />
              </a>
              <h6 class="mb-0">Company</h6>
            </div>
            <div>
              <router-link to="/" class="assign-user">
                <img :src="Ellipse4" alt="Ellipse4" class="img-fluid" />
              </router-link>
            </div>
          </div>
        </td>
        <td colspan="3">
          <div class="progress custom-progress-bar">
            <div
              class="progress-bar"
              role="progressbar"
              style="width: 25%"
              aria-valuenow="25"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
        </td>
      </tr>

      <tr>
        <td>
          <div
            class="d-flex sub-title align-items-center p-0 bg-transparent justify-content-between"
          >
            <div class="d-flex align-items-center gap-2">
              <a href="#">
                <img :src="PlusSign" alt="PlusSign" />
              </a>
              <h6 class="mb-0">CMS</h6>
            </div>
            <div>
              <router-link to="/" class="assign-user">
                <img :src="Image16" alt="Image16" class="img-fluid" />
              </router-link>
            </div>
          </div>
        </td>
        <td colspan="3">
          <div class="progress custom-progress-bar">
            <div
              class="progress-bar"
              role="progressbar"
              style="width: 30%"
              aria-valuenow="30"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
        </td>
      </tr>

      <tr>
        <td>
          <div class="d-flex align-items-center p-0 bg-transparent justify-content-between">
            <div class="d-flex align-items-center gap-2">
              <a href="#">
                <img :src="PlusSign" alt="PlusSign" />
              </a>
              <h6 class="mb-0">Jobulus</h6>
            </div>
            <div>
              <router-link to="/" class="assign-user">
                <img :src="Image16" alt="Image16" class="img-fluid" />
              </router-link>
              <router-link to="/" class="assign-user">
                <img :src="Ellipse4" alt="Ellipse4" class="img-fluid" />
              </router-link>
              <router-link to="/" class="assign-user">
                <img :src="Ellipse5" alt="Ellipse5" class="img-fluid" />
              </router-link>
            </div>
          </div>
        </td>
        <td colspan="3">
          <div class="progress custom-progress-bar">
            <div
              class="progress-bar"
              role="progressbar"
              style="width: 50%"
              aria-valuenow="50"
              aria-valuemin="0"
              aria-valuemax="100"
            ></div>
          </div>
        </td>
      </tr>
    </table>
  </div>
</template>

<style scoped>
.working-status-tble-wrap {
  border-radius: 8px;
  border: 1px solid #d4e1e4;
}
.Multi-Nested-sub-title {
  padding-left: 60px !important;
}
.sub-title {
  padding-left: 20px !important;
}
.Nested-sub-title {
  padding-left: 40px !important;
}
.assign-user:nth-child(1) {
  margin-left: 0px;
}
.assign-user {
  margin-left: -10px;
}
.working-status-tble {
  border-collapse: collapse;
}
.working-status-tble tr th {
  background-color: #f4f8f9;
  font-family: 'Poppins', sans-serif;
  font-size: 16px;
  font-weight: 500;
  color: #4f4f4f;
  padding: 20px;
  border: 1px solid #d4e1e4;
}
.working-status-tble tr td:nth-child(1) {
  border-right: 1px solid #d4e1e4;
}
.working-status-tble tr td {
  padding: 8px;
}
.working-status-tble tr:nth-child(odd) {
  background-color: #f4f8f9;
}
.custom-progress-bar {
  background-color: transparent;
  border-radius: 5px !important;
  padding: 15px;
  display: flex;
  align-items: center;
}
.progress-bar {
  display: flex;
  flex-direction: column;
  justify-content: center;
  overflow: hidden;
  text-align: center;
  white-space: nowrap;
  background-color: #3cc553;
  height: 30px;
  border-radius: 5px;
  align-items: center;
}
</style>
