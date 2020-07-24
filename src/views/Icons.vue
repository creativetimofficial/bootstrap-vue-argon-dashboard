<template>
  <div>
       <!-- BootstrapVue Done -->
    <base-header class="pb-6 pb-8 pt-5 pt-md-8 bg-gradient-success">
      <!-- Card stats -->
      <b-row>
        <b-col xl="3" md="6">
          <stats-card title="Total traffic"
                      type="gradient-red"
                      sub-title="350,897"
                      icon="ni ni-active-40"
                      class="mb-4">

            <template slot="footer">
              <span class="text-success mr-2">3.48%</span>
              <span class="text-nowrap">Since last month</span>
            </template>
          </stats-card>
        </b-col>
        <b-col xl="3" md="6">
          <stats-card title="Total traffic"
                      type="gradient-orange"
                      sub-title="2,356"
                      icon="ni ni-chart-pie-35"
                      class="mb-4">

            <template slot="footer">
              <span class="text-success mr-2">12.18%</span>
              <span class="text-nowrap">Since last month</span>
            </template>
          </stats-card>
        </b-col>
        <b-col xl="3" md="6">
          <stats-card title="Sales"
                      type="gradient-green"
                      sub-title="924"
                      icon="ni ni-money-coins"
                      class="mb-4">

            <template slot="footer">
              <span class="text-danger mr-2">5.72%</span>
              <span class="text-nowrap">Since last month</span>
            </template>
          </stats-card>

        </b-col>
        <b-col xl="3" md="6">
          <stats-card title="Performance"
                      type="gradient-info"
                      sub-title="49,65%"
                      icon="ni ni-chart-bar-32"
                      class="mb-4">

            <template slot="footer">
              <span class="text-success mr-2">54.8%</span>
              <span class="text-nowrap">Since last month</span>
            </template>
          </stats-card>
        </b-col>
      </b-row>
    </base-header>

    <b-container fluid class="mt--7">
      <b-row class="justify-content-center">
        <b-col lg="12">
          <card header-classes="bg-transparent">
            <h3 slot="header" class="mb-0">Icons</h3>
            <b-row class="icon-examples">
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-active-40'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-active-40"></i>
                    <span>active-40</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-air-baloon'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-air-baloon"></i>
                    <span>air-baloon</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-album-2'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-album-2"></i>
                    <span>album-2</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-align-center'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-align-center"></i>
                    <span>align-center</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-align-left-2'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-align-left-2"></i>
                    <span>align-left-2</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-ambulance'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-ambulance"></i>
                    <span>ambulance</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-app'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-app"></i>
                    <span>app</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-archive-2'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-archive-2"></i>
                    <span>archive-2</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-atom'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-atom"></i>
                    <span>atom</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-badge'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-badge"></i>
                    <span>badge</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-bag-17'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-bag-17"></i>
                    <span>bag-17</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-basket'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-basket"></i>
                    <span>basket</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-bell-55'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-bell-55"></i>
                    <span>bell-55</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-bold-down'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-bold-down"></i>
                    <span>bold-down</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-bold-left'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-bold-left"></i>
                    <span>bold-left</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-bold-right'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-bold-right"></i>
                    <span>bold-right</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-bold-up'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-bold-up"></i>
                    <span>bold-up</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-bold'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-bold"></i>
                    <span>bold</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-book-bookmark'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-book-bookmark"></i>
                    <span>book-bookmark</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-books'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-books"></i>
                    <span>books</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-box-2'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-box-2"></i>
                    <span>box-2</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-briefcase-24'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-briefcase-24"></i>
                    <span>briefcase-24</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-building'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-building"></i>
                    <span>building</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-bulb-61'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-bulb-61"></i>
                    <span>bulb-61</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-bullet-list-67'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-bullet-list-67"></i>
                    <span>bullet-list-67</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-bus-front-12'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-bus-front-12"></i>
                    <span>bus-front-12</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-button-pause'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-button-pause"></i>
                    <span>button-pause</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-button-play'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-button-play"></i>
                    <span>button-play</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-button-power'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-button-power"></i>
                    <span>button-power</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-calendar-grid-58'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-calendar-grid-58"></i>
                    <span>calendar-grid-58</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-camera-compact'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-camera-compact"></i>
                    <span>camera-compact</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-caps-small'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-caps-small"></i>
                    <span>caps-small</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-cart'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-cart"></i>
                    <span>cart</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-chart-bar-32'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-chart-bar-32"></i>
                    <span>chart-bar-32</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-chart-pie-35'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-chart-pie-35"></i>
                    <span>chart-pie-35</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-chat-round'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-chat-round"></i>
                    <span>chat-round</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-check-bold'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-check-bold"></i>
                    <span>check-bold</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-circle-08'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-circle-08"></i>
                    <span>circle-08</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-cloud-download-95'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-cloud-download-95"></i>
                    <span>cloud-download-95</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-cloud-upload-96'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-cloud-upload-96"></i>
                    <span>cloud-upload-96</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-compass-04'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-compass-04"></i>
                    <span>compass-04</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-controller'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-controller"></i>
                    <span>controller</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-credit-card'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-credit-card"></i>
                    <span>credit-card</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-curved-next'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-curved-next"></i>
                    <span>curved-next</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-delivery-fast'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-delivery-fast"></i>
                    <span>delivery-fast</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-diamond'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-diamond"></i>
                    <span>diamond</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-email-83'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-email-83"></i>
                    <span>email-83</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-fat-add'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-fat-add"></i>
                    <span>fat-add</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-fat-delete'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-fat-delete"></i>
                    <span>fat-delete</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-fat-remove'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-fat-remove"></i>
                    <span>fat-remove</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-favourite-28'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-favourite-28"></i>
                    <span>favourite-28</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-folder-17'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-folder-17"></i>
                    <span>folder-17</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-glasses-2'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-glasses-2"></i>
                    <span>glasses-2</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-hat-3'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-hat-3"></i>
                    <span>hat-3</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-headphones'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-headphones"></i>
                    <span>headphones</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-html5'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-html5"></i>
                    <span>html5</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-istanbul'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-istanbul"></i>
                    <span>istanbul</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-circle-08'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-circle-08"></i>
                    <span>circle-08</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-key-25'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-key-25"></i>
                    <span>key-25</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-laptop'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-laptop"></i>
                    <span>laptop</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-like-2'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-like-2"></i>
                    <span>like-2</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-lock-circle-open'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-lock-circle-open"></i>
                    <span>lock-circle-open</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-map-big'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-map-big"></i>
                    <span>map-big</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-mobile-button'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-mobile-button"></i>
                    <span>mobile-button</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-money-coins'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-money-coins"></i>
                    <span>money-coins</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-note-03'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-note-03"></i>
                    <span>note-03</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-notification-70'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-notification-70"></i>
                    <span>notification-70</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-palette'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-palette"></i>
                    <span>palette</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-paper-diploma'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-paper-diploma"></i>
                    <span>paper-diploma</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-pin-3'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-pin-3"></i>
                    <span>pin-3</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-planet'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-planet"></i>
                    <span>planet</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-ruler-pencil'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-ruler-pencil"></i>
                    <span>ruler-pencil</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-satisfied'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-satisfied"></i>
                    <span>satisfied</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-scissors'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-scissors"></i>
                    <span>scissors</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-send'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-send"></i>
                    <span>send</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-settings-gear-65'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-settings-gear-65"></i>
                    <span>settings-gear-65</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-settings'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-settings"></i>
                    <span>settings</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-single-02'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-single-02"></i>
                    <span>single-02</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-single-copy-04'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-single-copy-04"></i>
                    <span>single-copy-04</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-sound-wave'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-sound-wave"></i>
                    <span>sound-wave</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-spaceship'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-spaceship"></i>
                    <span>spaceship</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-square-pin'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-square-pin"></i>
                    <span>square-pin</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-support-16'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-support-16"></i>
                    <span>support-16</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-tablet-button'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-tablet-button"></i>
                    <span>tablet-button</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-tag'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-tag"></i>
                    <span>tag</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-tie-bow'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-tie-bow"></i>
                    <span>tie-bow</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-time-alarm'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-time-alarm"></i>
                    <span>time-alarm</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-trophy'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-trophy"></i>
                    <span>trophy</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-tv-2'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-tv-2"></i>
                    <span>tv-2</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-umbrella-13'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-umbrella-13"></i>
                    <span>umbrella-13</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-user-run'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-user-run"></i>
                    <span>user-run</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-vector'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-vector"></i>
                    <span>vector</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-watch-time'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-watch-time"></i>
                    <span>watch-time</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-world'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-world"></i>
                    <span>world</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-zoom-split-in'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-zoom-split-in"></i>
                    <span>zoom-split-in</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-collection'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-collection"></i>
                    <span>collection</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-image'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-image"></i>
                    <span>image</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-shop'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-shop"></i>
                    <span>shop</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-ungroup'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-ungroup"></i>
                    <span>ungroup</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-world-2'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-world-2"></i>
                    <span>world-2</span>
                  </div>
                </button>
              </b-col>
              <b-col lg="3" md="6">
                <button type="button" class="btn-icon-clipboard" v-clipboard:copy="'ni ni-ui-04'"
                        v-clipboard:success="onCopy"
                        title=""
                        data-original-title="Copy to clipboard">
                  <div>
                    <i class="ni ni-ui-04"></i>
                    <span>ui-04</span>
                  </div>
                </button>
              </b-col>

            </b-row>
          </card>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>
<script>
  import Vue from 'vue'
  import VueClipboard from 'vue-clipboard2'
  import BaseHeader from '@/components/BaseHeader';

  Vue.use(VueClipboard)
  export default {
    name: 'icons',
    components: {
      BaseHeader
    },
    methods: {
      onCopy() {
        this.$notify({
          type: 'info',
          message: 'Copied to clipboard'
        })
      }
    }
  };
</script>
<style></style>
