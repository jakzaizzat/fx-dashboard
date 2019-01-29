<template>
    <div class="font-sans bg-grey-lighter flex flex-col min-h-screen">
  <div>
    <div class="bg-blue-dark">
      <div class="container mx-auto px-4">
        <div class="flex items-center md:justify-between py-4">
          <div class="w-1/4 md:hidden">
            <svg class="fill-current text-white h-8 w-8" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M16.4 9H3.6c-.552 0-.6.447-.6 1 0 .553.048 1 .6 1h12.8c.552 0 .6-.447.6-1 0-.553-.048-1-.6-1zm0 4H3.6c-.552 0-.6.447-.6 1 0 .553.048 1 .6 1h12.8c.552 0 .6-.447.6-1 0-.553-.048-1-.6-1zM3.6 7h12.8c.552 0 .6-.447.6-1 0-.553-.048-1-.6-1H3.6c-.552 0-.6.447-.6 1 0 .553.048 1 .6 1z"/></svg>
          </div>
          <div class="w-1/2 md:w-auto text-center text-white text-2xl font-medium tracking-wide">
            FX
          </div>
        </div>
      </div>
    </div>
  </div>

  <div class="flex-grow container mx-auto sm:px-4 pt-6 pb-8">
    <div class="flex flex-wrap -mx-4">
      <div class="w-full mb-6 lg:mb-0 px-4 flex flex-col">
        <div class="flex-grow flex flex-col bg-white border-t border-b sm:rounded sm:border shadow overflow-hidden">
          <div class="border-b">
            <div class="flex justify-between px-6 -mb-px">
              <h3 class="text-blue-dark py-4 font-normal text-lg">Intra Close</h3>
            </div>
          </div>

          <div class="flex px-6 py-4 text-grey-darker bg-grey-lighter items-center border-b -mx-4 text-sm">
            <div class="w-2/5 xl:w-1/4 px-4 flex items-center">
              <div class="rounded-full bg-orange inline-flex mr-3">
              </div>
              <span class="text-sm">Pair</span>
            </div>
            <div class="md:flex xl:flex w-1/4 px-4 items-center">
              Price
            </div>
            <div class="flex w-3/5 md:w/12">
              <div class="w-1/2 px-4">
                <div class="text-right">
                  TP
                </div>
              </div>
              <div class="w-1/2 px-4">
                <div class="text-right text-grey">
                  SL
                </div>
              </div>
            </div>
          </div>

          <div v-for="signal in intraClose" :key="signal.id" class="flex px-6 py-6 text-grey-darker items-center border-b -mx-4">
            <div class="w-2/5 xl:w-1/4 px-4 flex items-center">
              <div class="rounded-full bg-orange inline-flex mr-3">
              </div>
              <span class="tracking-wide">{{ signal.counter_signal.name }} <span :class="{ 'text-green': signal.pip_result === 'TP', 'text-red': signal.pip_result === 'SL' }">{{ signal.pip }}</span></span>
            </div>
            <div class="md:flex xl:flex flex-col w-1/4 px-4 items-start">
              <p class="mb-1 text-xs" :class="{ 'text-blue': signal.action_signal.name === 'BUY', 'text-red': signal.action_signal.name === 'SELL' }">{{ signal.action_signal.name }}</p>
              {{ signal.price }}
            </div>
            <div class="flex w-3/5 md:w/12">
              <div class="w-1/2 px-4">
                <div class="text-right">
                  {{ signal.target_price }}
                </div>
              </div>
              <div class="w-1/2 px-4">
                <div class="text-right text-grey">
                  {{ signal.stop_loss }}
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
import axios from 'axios'
export default {
    data() {
        return {
            intraOpen: [],
            swingOpen: [],
            intraClose: [],
        }
    },
    methods: {
        fetchIntraClose() {
            // Get all transactions
            axios.get(`http://admin.overpips.com/public/api/v1/intra_closed`)
            .then(res=>{
                this.intraClose = res.data.data;
            })
            .catch(err => {
            console.log(err);
            });
        }
    },
    created() {
        this.fetchIntraClose();
    }
}
</script>

